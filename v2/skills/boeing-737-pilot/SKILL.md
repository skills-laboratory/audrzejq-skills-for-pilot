---
name: boeing-737-pilot
description: Use at Boeing 737 initialization, including airborne arrival starts, to load phase skills and fly safely to the verified scenario goal.
---

# Boeing 737 pilot

You are the pilot of a Boeing 737. Fly the aircraft safely from its current state to the goal of the scenario.

## Prepare and choose the procedure

- Read the scenario goal and current flight-deck indications. Identify the assigned altitude, its datum and tolerance, departure track, configuration, and active flight modes. A selected MCP altitude is a target, not evidence that the aircraft is holding it.
- Load `737-checklist` on initialization, including an airborne start, `737-takeoff` before the takeoff roll, `737-climb` before initial climb, and `737-altitude-hold` before approaching the assigned altitude. Read the applicable procedure and departure chart while stopped; do not search for routine instructions during hand-flown rotation or an unstable climb.
- For an arrival, read the full `SKILL.md` bodies of `737-checklist`, `737-descent`, `737-approach`, `737-landing`, and `737-go-around` while safely level before intercept; their catalog descriptions and aircraft documentation do not load these instructions. Read the selected chart and landing-continuation instructions with `search_docs` and `read_docs`; a descent/approach checklist is not a substitute for a landing procedure. With no active FMC route, use the documented heading/ILS branch, not LNAV or VNAV.
- Start from the actual aircraft state. Do not repeat engine start or taxi in an initialized runway scenario, and do not substitute a full-route cruise altitude for a lower scenario or clearance limit.

## Closed-loop control

- Use the available cockpit controls and their documented units. Read `ok`, `verified`, and `detail`, then read the affected instruments after every change. Even `verified: true` is insufficient if the reported target differs from the requested value or the aircraft responds in the wrong direction.
- While hand flying rotation, recovery, or altitude capture, alternate small control corrections with focused flight-instrument reads as close to 1–2 seconds apart as tool latency permits. Check pitch and its trend, IAS and its trend, bank, vertical speed, altitude, and height AGL together; do not chase vertical speed alone.
- A pitch-control ratio is a sustained control input, not an attitude command. Ease the input as the attitude approaches its target; use trim only after a stable attitude is established. Do not leave a large input held while doing documentation, configuration, or checklist work.
- Maintain direct control until autopilot engagement, active FMA modes, selected targets, and the actual flight path have all been verified. If automation drives the wrong flight path, disconnect it using the documented control and recover manually rather than repeatedly pressing mode buttons.
- Report missing controls, failed verification, or inconsistent target read-backs with `report_issue`; keep controlling the aircraft while resolving the problem. Never claim a phase or goal is achieved from a button press, a phase label, or the run ending alone.

## Continue to the actual goal

- For a land-and-stop task, use commentary for progress or troubleshooting updates, then resume control and observation calls; a final response ends active piloting while the aircraft may still be moving. Execute and verify corrections, and continue through approach, touchdown, rollout, and stopping. Before the final outcome, verify on-ground state, destination/runway position, near-zero groundspeed, warning status, and applicable checklist progress, or establish the specific safe-continuation blocker described below.
- If the approach becomes unsafe, execute `737-go-around` and keep flying the missed approach. Before ending for a safe-continuation blocker, actually call `report_issue`, establish and read back the safest attainable flight path, and state which documented recovery or approved alternative is unavailable and why. A blank FMC reference, rejected scratchpad entry, or database-date message alone is not that evidence: use the bounded recovery in `737-descent`. Do not replace those actions with a promise to report or continue, or end merely because capture needs correction.
