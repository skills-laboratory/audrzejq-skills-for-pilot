---
name: 737-takeoff
description: Use for runway preparation, takeoff roll, rotation, and initial gear retraction in the Boeing 737-800.
---

# Boeing 737 takeoff

## Before advancing thrust

- Read the applicable takeoff procedure, live checklist, and `737-climb` while stopped. Establish the departure track, assigned altitude, initial climb speed, acceleration conditions, actual flap-retraction detents/speeds, and autoflight plan before releasing the brakes; do not leave the retraction schedule for an airborne search.
- Obtain V1, VR, V2, takeoff thrust, flap detent, and trim from the configured FMC/performance data for the actual weight and conditions. Distinguish suggested values from entered/confirmed values. Do not use a remembered fixed rotation speed.
- Verify flap configuration, gear down, speedbrake down, trim, brakes, required lights, transponder, and runway/takeoff authority. Set and read back the assigned MCP altitude and the procedure's takeoff speed/heading; do not leave initialized speed or heading defaults in place.
- For a normal flight-director/autothrottle takeoff, verify flight director ON and autothrottle ARM in `mcp-and-autopilot` before TO/GA. If either is OFF, use its documented control and read it back; toggle only after checking the current state. A runway-loaded aircraft need not have these prerequisites enabled. Arming does not establish an active mode.

## Roll and rotate

1. With braking verified, adjust thrust toward approximately 40% measured N1 on both engines. The throttle control sets lever percentage, not N1: confirm the lever read-back, allow engine spool-up to settle, then make small lever corrections from measured N1 and its trend. If stabilized N1 is too high, reduce the levers; matched engines alone do not establish the requested N1. After stabilization, push TO/GA once as prescribed and read engine and FMA indications to confirm the intended takeoff thrust/modes. Release the brakes for the roll only with the required setup verified.
2. Maintain centerline with small directional corrections and monitor IAS, acceleration, and engine symmetry. Near VR, use focused instrument reads rather than documentation searches.
3. At the confirmed VR, rotate smoothly toward approximately 15° at about 2–3° per second. Read flight instruments immediately after the pitch command, aiming for 1–2 second feedback without deliberate waits. Around 10°, move the rotation input toward neutral rather than merely halving a positive ratio and leaving it held. Estimate time remaining to the target as remaining degrees divided by observed pitch rate; include reading, decision, and control-call delay before the next correction. If that delay consumes the remaining time, remove the rotation input now. Neutral is not an attitude lock: if pitch still rises toward an overshoot, use a brief, small nose-down correction and read the response immediately. Stabilize actual pitch and its trend, not the yoke ratio.
4. After liftoff, follow valid flight-director guidance and the procedure's initial climb speed, normally V2 plus its specified margin. If pitch continues above the target or IAS falls toward V2, reduce back-pressure immediately and check the response; do not hold the rotation input to obtain a larger climb rate.
5. Confirm airborne state and positive climb from rising altitude and positive vertical speed before selecting gear UP. Before the gear call, ease rotation input as needed from the latest pitch trend; do not leave back-pressure unchanged while attending to the gear. Read pitch and IAS immediately after the selection, and interleave flight-instrument reads with gear-transit verification through completion. Continue with `737-climb`.

Record each verified checklist action using `737-checklist`. Do not let marking, gear reads, or roll-mode selection interrupt pitch and IAS control.

## If TO/GA has no response

While stopped, reduce thrust to idle and verify braking before troubleshooting. Recheck flight director ON, autothrottle ARM, selected targets, and the documented takeoff prerequisites; correct an omitted prerequisite and read it back before a further prescribed TO/GA attempt. Do not repeat the command in an unchanged setup or declare a tool fault from a blank FMA alone. If the response remains absent, call `report_issue` and use manual thrust only under an explicitly documented procedure branch with verified thrust and a safe flight-control plan; otherwise remain stopped at idle and explain the unresolved safety prerequisite.
