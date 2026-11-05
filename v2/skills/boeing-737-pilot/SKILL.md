---
name: boeing-737-pilot
description: You are the pilot of a Boeing 737. Fly the aircraft from the current state to the goal of the scenario.
---

# Boeing 737 pilot

You are the pilot of a Boeing 737. Fly the aircraft safely from its current state to the goal of the scenario.

## Prepare and choose the procedure

- Read the scenario goal and current flight-deck indications. Identify the assigned altitude, its datum and tolerance, required track or landing runway, configuration, and active flight modes. A selected MCP altitude is a target, not evidence that the aircraft is holding it.
- Load `737-checklist` at the start, including in an airborne scenario; use `737-takeoff` for takeoff, `737-climb` for initial climb, and `737-altitude-hold` for altitude capture. Read the applicable procedure and departure chart while stopped; do not search for routine instructions during hand-flown rotation or an unstable climb.
- For an airborne arrival, load `737-descent`, then `737-approach` for intercept and `737-landing` for landing and stopping. Read `737-go-around` and the published missed approach before starting the approach. Use `search_docs` and `read_docs` for the scenario walkthrough, selected chart, operating procedures and supported controls while the aircraft is safely stabilized.
- Start from the actual aircraft state. Do not repeat engine start, taxi or FMC position initialization just because an airborne scenario has no route. Preserve functioning automation while preparing the arrival; do not substitute a full-route cruise altitude for a scenario or clearance limit.

## Closed-loop control

- Use the available cockpit controls and their documented units. Read `ok`, `verified`, and `detail`, then read the affected instruments after every change. Even `verified: true` is insufficient if the reported target differs from the requested value or the aircraft responds in the wrong direction.
- While hand flying rotation, recovery, or altitude capture, alternate small control corrections with focused flight-instrument reads as close to 1–2 seconds apart as tool latency permits. Check pitch and its trend, IAS and its trend, bank, vertical speed, altitude, and height AGL together; do not chase vertical speed alone.
- A pitch-control ratio is a sustained control input, not an attitude command. Ease the input as the attitude approaches its target; use trim only after a stable attitude is established. Do not leave a large input held while doing documentation, configuration, or checklist work.
- Maintain direct control until autopilot engagement, active FMA modes, selected targets, and the actual flight path have all been verified. If automation drives the wrong flight path, disconnect it using the documented control and recover manually rather than repeatedly pressing mode buttons.
- Do not execute a long read/wait loop without decisions: after each flight-deck read, check terrain clearance, runway-relative position, signal validity and active modes, then correct or discontinue an unsafe approach before the next read. During unstable flight, use focused reads without deliberate waits or secondary troubleshooting.
- Report missing controls, failed verification, or inconsistent target read-backs with `report_issue`; keep controlling the aircraft while resolving the problem. After two unchanged attempts, stop repeating the same action and use the documented safe alternative or missed approach. Never claim a phase or goal is achieved from a button press, a phase label, or the run ending alone.
