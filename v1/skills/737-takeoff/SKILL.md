---
name: 737-takeoff
description: Use for runway preparation, takeoff roll, rotation, and initial gear retraction in the Boeing 737-800.
---

# Boeing 737 takeoff

## Before advancing thrust

- Read the detailed takeoff procedure, live checklist, and `737-climb` while stopped; a scenario overview or route example does not replace the operating procedure. Establish the departure track, assigned altitude, initial climb speed, acceleration conditions, actual flap-retraction detents/speeds, and autoflight plan before releasing the brakes; do not leave the retraction schedule for an airborne search.
- Obtain V1, VR, V2, takeoff thrust, flap detent, and trim from the configured FMC/performance data for the actual weight and conditions. Distinguish suggested values from entered/confirmed values. Do not use a remembered fixed rotation speed.
- Verify flap configuration, gear down, speedbrake down, trim, brakes, required lights, transponder, and runway/takeoff authority. Set and read back the assigned MCP altitude and the procedure's takeoff speed/heading. Establish the prescribed flight-director and autothrottle configuration. When using automatic takeoff thrust, explicitly verify autothrottle ARM before TO/GA; the flight director alone cannot advance thrust, and arming does not establish an active mode.

## Roll and rotate

1. Advance thrust to approximately 40% measured N1 on both engines and verify stabilization, not just a transient crossing during spool-up; 40% thrust-lever position is not 40% N1. Keep brakes applied during standing-takeoff preparation. Push TO/GA once as prescribed, then verify actual N1 against the planned takeoff thrust and read the active FMA modes. An unverified button response, blank thrust FMA, or unchanged thrust levers is not proof of automatic takeoff thrust. Resolve the response using the documented automatic or manual thrust procedure before committing to the roll. If already rolling when a thrust failure is identified, follow the applicable rejected-takeoff criteria and V1 limitations rather than attempting rotation on unresolved thrust.
2. Maintain centerline with small directional corrections and monitor IAS, acceleration, and engine symmetry. Do not preload nose-up input before the observed VR or increase it because pitch barely changes on the ground: the wheels constrain attitude, and that input can become excessive after liftoff. Near VR, use focused instrument reads rather than documentation searches.
3. At the confirmed VR, rotate smoothly toward approximately 15° at about 2–3° per second, using the smallest input that establishes the intended rate. Read flight instruments immediately after the pitch command, aiming for 1–2 second feedback without deliberate waits. Around 10°, move the rotation input toward neutral rather than merely halving a positive ratio and leaving it held. Estimate time remaining to the target as remaining degrees divided by observed pitch rate; include reading, decision, and control-call delay before the next correction. If that delay consumes the remaining time, remove the rotation input now. If already above the target and still pitching up, remove positive input immediately; do not wait for IAS to fall. Neutral is not an attitude lock: if pitch still rises toward an overshoot, use a brief, small nose-down correction and read the response immediately. Stabilize actual pitch and its trend, not the yoke ratio.
4. After liftoff, follow valid flight-director guidance and the procedure's initial climb speed, normally V2 plus its specified margin. If pitch continues above the target or IAS falls toward V2, reduce back-pressure immediately and check the response; do not hold the rotation input to obtain a larger climb rate.
5. Confirm airborne state and positive climb from rising altitude and positive vertical speed before selecting gear UP. Before the gear call, ease rotation input as needed from the latest pitch trend; do not leave back-pressure unchanged while attending to the gear. Read pitch and IAS immediately after the selection, and interleave flight-instrument reads with gear-transit verification through completion. Continue with `737-climb`.

Record each verified checklist action using `737-checklist`. Do not let marking, gear reads, or roll-mode selection interrupt pitch and IAS control.
