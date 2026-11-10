---
name: 737-arrival
description: Use for airborne arrival preparation, FMC entry problems, and monitored ILS interception in the Boeing 737-800.
---

# Boeing 737 arrival

## Protect the approach before troubleshooting

1. Read actual altitude, IAS, ground speed, position, configuration and FMA. Read the assigned approach chart and landing-continuation procedure; establish the intercept altitude, minimums, missed approach and configuration schedule. A phase label or selected altitude does not establish approach readiness.
2. Tune and identify the approach receivers and set their courses early, so valid DME and localizer/glideslope indications are available before prolonged FMC work. Set and verify QNH, minimums, lights, passenger signs and autobrake against the applicable procedure.
3. Before each documentation or CDU task, read distance, IAS, altitude, deviations and FMA. Estimate time to the next charted intercept or configuration point as distance remaining divided by ground speed, converting hours to seconds; allow for tool and decision latency. If the task would consume that margin, defer troubleshooting and manage the flight path now.
4. Interleave each CDU entry-and-verification cycle with focused flight/approach reads. When interception or configuration becomes imminent, stop secondary tasks and monitor capture continuously. If unprepared, above the glidepath or unable to stabilize, use the authorized hold, repositioning or missed-approach procedure; do not attempt a steep catch-up descent close to the runway.

## Prepare and verify the landing reference

- Obtain VREF and the approach-speed correction from documented performance data for actual weight and selected landing flaps; do not substitute a guessed speed or takeoff V-speeds.
- Read the CDU title, labels, units and scratchpad before entry. Clear an error or residual text using the documented CLR operation and verify an empty scratchpad before typing a replacement; otherwise successive attempts can concatenate. Use only the documented field and format, then read the displayed result, not just the key-press acknowledgement.
- If a correctly formatted entry is rejected, check the documented prerequisites and make one corrected retry only when there is new evidence and sufficient flight-path margin. Repeatedly trying different weights, units or line-select keys is not a recovery procedure. Report the limitation and preserve approach monitoring.
- An unavailable FMC field is a tool/setup limitation, not permission to claim VREF entry. Use an independently supported landing-performance source if available; otherwise report the missing data and do not continue an approach that cannot be supported safely.
- Verify selected pressurization landing altitude against the destination requirement; current cabin altitude is not that selection. For annunciator recall, identify the illuminated system and inspect its source indications before acknowledgement. A reset master caution does not prove the underlying condition is resolved.

## Intercept and configure

- Distinguish APP armed, localizer captured, glideslope alive and glideslope captured using valid receiver indications and active/armed FMA. Intercept from the charted safe altitude below the glidepath; do not assume centered pointers with no station identification are valid guidance.
- Follow the landing procedure's gear, flap, start-switch and speedbrake sequence at the observed triggers. Verify three green, actual flap travel, safe maneuver speed and SPEEDBRAKE ARMED before recording the corresponding checks with `737-checklist`.
- After glideslope capture, verify active G/S and descent, select landing flaps and the missed-approach altitude as prescribed, and read the resulting targets. For autoland, verify the documented dual-channel prerequisites and landing modes; do not disturb a verified capture merely because a mode button is unlit.
- Evaluate conditional checklist items explicitly. A normal landing-flap choice does not call for flaps-15 GPWS inhibit; an RNP update depends on the selected procedure. Record supported not-applicable status with its evidence, or report that the interface cannot represent it; never inhibit warnings or mark an unperformed action simply to fill the checklist.
