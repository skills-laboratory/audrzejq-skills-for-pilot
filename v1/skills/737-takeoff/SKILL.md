---
name: 737-takeoff
description: Use for runway preparation, takeoff roll, rotation, and initial gear retraction in the Boeing 737-800.
---

# Boeing 737 takeoff

## Before advancing thrust

- Read the applicable takeoff procedure, live checklist, and `737-climb` while stopped. Establish the departure track, assigned altitude, initial climb speed, acceleration conditions, actual flap-retraction detents/speeds, and autoflight plan before releasing the brakes; do not leave the retraction schedule for an airborne search.
- Obtain V1, VR, V2, takeoff thrust, flap detent, and trim from the configured FMC/performance data for the actual weight and conditions. Distinguish suggested values from entered/confirmed values. Do not use a remembered fixed rotation speed.
- Verify flap configuration, gear down, speedbrake down, trim, brakes, required lights, transponder, and runway/takeoff authority. Set and read back the assigned MCP altitude and the procedure's takeoff speed/heading. Establish the prescribed flight-director and autothrottle configuration; arming does not establish an active mode.

## Roll and rotate

1. Advance thrust to approximately 40% N1 on both engines and verify stabilization, using measured N1 rather than thrust-lever percentage. Push TO/GA once as prescribed; read engine and FMA indications to confirm the intended takeoff thrust/modes. Resolve an unverified TO/GA response before assuming takeoff thrust is established.
2. Maintain centerline with small directional corrections and monitor IAS, acceleration, and engine symmetry. Near VR, use focused instrument reads rather than documentation searches.
3. At the confirmed VR, rotate smoothly toward approximately 15° at about 2–3° per second, then immediately read `flight-instruments`. Use the measured read–decision–control interval from `boeing-737-pilot` to project pitch before the next correction. Release toward neutral before that projection reaches 15°; with slow feedback this can require release before 10°, not waiting to observe 10° or 15°. Merely halving a positive ratio still commands nose-up. If pitch continues rising after release, use a brief, small counter-correction and immediately read back the response. Arrest the pitch rate before marking rotation complete or attending to secondary tasks.
4. After liftoff, follow valid flight-director guidance and the procedure's initial climb speed, normally V2 plus its specified margin. If pitch continues above the target or IAS falls toward V2, reduce back-pressure immediately and check the response; do not hold the rotation input to obtain a larger climb rate.
5. Confirm airborne state and positive climb from rising altitude and positive vertical speed before selecting gear UP. Before the gear call, ease rotation input as needed from the latest pitch trend; do not leave back-pressure unchanged while attending to the gear. Read pitch and IAS immediately after the selection, and interleave flight-instrument reads with gear-transit verification through completion. Continue with `737-climb`.

Record each verified checklist action using `737-checklist`. Do not let marking, gear reads, or roll-mode selection interrupt pitch and IAS control.
