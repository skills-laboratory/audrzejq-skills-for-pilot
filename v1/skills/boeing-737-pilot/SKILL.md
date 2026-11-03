---
name: boeing-737-pilot
description: Use at the start of every Boeing 737 flight, before movement or thrust changes, to load phase procedures and verify readiness; continue using it to coordinate safe flight to the scenario goal.
---

# Boeing 737 pilot

You are the pilot of a Boeing 737. Fly the aircraft safely from its current state to the goal of the scenario.

## Prepare and verify readiness

- Read the scenario goal and current flight-deck indications. Identify the assigned altitude, its datum and tolerance, departure track, configuration, and active flight modes. A selected MCP altitude is a target, not evidence that the aircraft is holding it.
- While stopped, load `737-checklist`, `737-takeoff`, `737-climb`, and `737-altitude-hold`, and read the applicable procedure and departure chart. A skill description is not the loaded procedure. Prepare capture as well as takeoff before releasing the brakes; do not search for routine instructions during hand-flown rotation or an unstable climb.
- Start from the actual aircraft state. Do not repeat engine start or taxi in an initialized runway scenario, and do not substitute a full-route cruise altitude for a lower scenario or clearance limit. Engines running and a route loaded do not establish flight-director, autothrottle, or autopilot readiness.
- Before releasing the brakes, verify the assigned MCP altitude matches the scenario limit, confirmed takeoff performance and configuration, and the prescribed flight-director/autothrottle setup. Resolve missing prerequisites while stopped; a completed checklist section is not proof of these conditions. If controls or instructions are unavailable, report the limitation rather than beginning an unprepared roll.

## Closed-loop control

- Use the available cockpit controls and their documented units. Read `ok`, `verified`, and `detail`, then read the affected instruments after every change. Even `verified: true` is insufficient if the reported target differs from the requested value or the aircraft responds in the wrong direction.
- While hand flying rotation, recovery, or altitude capture, alternate small control corrections with focused flight-instrument reads, aiming for 1–2 second feedback. Check pitch and its trend, IAS and its trend, bank, vertical speed, altitude, and height AGL together; do not chase vertical speed alone.
- Use the observed interval between instrument reads, including decision and control-call time, not just the tool duration, to judge whether the next correction will arrive in time. If time to the attitude or altitude target is shorter than that interval, ease the sustained input now and check the response; do not leave it held through checklist or configuration calls. Plan a documented, permitted autoflight handoff when stable if manual feedback is too slow, and report the limitation; do not engage automation during an unsafe recovery.
- A pitch-control ratio is a sustained control input, not an attitude command. Ease the input as the attitude approaches its target; use trim only after a stable attitude is established. Do not leave a large input held while doing documentation, configuration, or checklist work.
- Maintain direct control until autopilot engagement, active FMA modes, selected targets, and the actual flight path have all been verified. If automation drives the wrong flight path, disconnect it using the documented control and recover manually rather than repeatedly pressing mode buttons.
- Report missing controls, failed verification, or inconsistent target read-backs with `report_issue`; keep controlling the aircraft while resolving the problem. Never claim a phase or goal is achieved from a button press, a phase label, or the run ending alone.
