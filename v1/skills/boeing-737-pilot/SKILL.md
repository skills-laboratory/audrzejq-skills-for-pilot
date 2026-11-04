---
name: boeing-737-pilot
description: You are the pilot of a Boeing 737. Fly the aircraft from the current state to the goal of the scenario.
---

# Boeing 737 pilot

You are the pilot of a Boeing 737. Fly the aircraft safely from its current state to the goal of the scenario.

## Prepare and choose the procedure

- Read the scenario goal and current flight-deck indications. Identify the assigned altitude, its datum and tolerance, departure track, configuration, and active flight modes. A selected MCP altitude is a target, not evidence that the aircraft is holding it.
- Load `737-checklist` before movement, `737-takeoff` before the takeoff roll, `737-climb` before initial climb, and `737-altitude-hold` before approaching the assigned altitude. Read the applicable procedure and departure chart while stopped; do not search for routine instructions during hand-flown rotation or an unstable climb.
- Start from the actual aircraft state. Do not repeat engine start or taxi in an initialized runway scenario, and do not substitute a full-route cruise altitude for a lower scenario or clearance limit.

## Closed-loop control

- Use the available cockpit controls and their documented units. Read `ok`, `verified`, and `detail`, then read the affected instruments after every change. Even `verified: true` is insufficient if the reported target differs from the requested value or the aircraft responds in the wrong direction.
- While hand flying rotation, recovery, or altitude capture, alternate small control corrections with `read_group` of `flight-instruments` as close to 1–2 seconds apart as tool latency permits. Check pitch, IAS, bank, heading, vertical speed, altitude, and height AGL together rather than omitting lateral control during separate reads. A neutral roll input does not guarantee wings level: correct unintended bank and heading drift with the documented roll control and verify the response; selected heading alone does not steer.
- A signed pitch-control ratio is a sustained control input, not an attitude command; neutral is 0, not a smaller positive or negative ratio. Estimate current pitch rate from successive pitch readings and elapsed time: an averaged trend may still include a previous command. Remove the input before the next read–decision–action cycle would pass the target, then use brief counter-corrections to damp remaining motion. Once attitude and IAS stabilize, trim in small verified increments to relieve sustained control pressure; do not leave a large input held during secondary tasks.
- Continued pitch motion after an opposing correction is not proof that the control sign is reversed: a slowing pitch rate can be normal braking rather than a sign reversal. Compare successive rates and actual axis input, trim, and active modes before changing the assumed control direction. If contradictory behavior persists, report it and keep the recovery bounded rather than escalating alternating inputs.
- Maintain direct control until a stable, trimmed handoff, documented axis/override management, persistent CMD engagement across successive reads, active FMA modes, selected targets, and actual flight path have all been verified. If CMD drops out, do not stack more mode/engagement calls while a recovery input remains held; stabilize manually and report the unresolved handoff. If automation drives the wrong flight path, disconnect it using the documented control and recover manually rather than repeatedly pressing mode buttons.
- Report missing controls, failed verification, or inconsistent target read-backs with `report_issue`; keep controlling the aircraft while resolving the problem. Never claim a phase or goal is achieved from a button press, a phase label, or the run ending alone.
