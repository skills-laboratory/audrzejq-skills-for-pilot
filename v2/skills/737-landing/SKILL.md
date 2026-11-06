---
name: 737-landing
description: Use on a captured, configured ILS for verified autoland or an authorized manual landing, touchdown, rollout, and stopping.
---

# Boeing 737 landing and rollout

## Verify the landing method before low final

1. Read the documented landing/autoland continuation before final. Confirm valid localizer and G/S capture, landing performance, gear three green, landing flaps, speedbrake arming, autobrake, and applicable minima. Continue recording observed conditions through `737-checklist`; do not let marking interrupt flight-path monitoring.
2. For the documented dual-channel autoland, with one CMD channel flying the coupled ILS and APP selected, engage the other through its supported hold action (`cmd-b-hold` with CMD A first, or `cmd-a-hold` with CMD B first). A short CMD press can exchange channels instead of establishing both. Engage promptly after capture, while above approximately 1,500 ft height AGL, and respect the documented radio-altitude lockout; terrain AGL is not a dedicated radio-altimeter indication.
3. Verify both CMD channels, active VOR/LOC and G/S, and the required armed FLARE/ROLLOUT modes. Observe the actual flight path as well as the annunciations. If a channel drops or FLARE has not armed by the documented 350 ft gate, go around rather than repeatedly pressing CMD or improvising a manual flare. An authorized change to a manual landing must be briefed and established above the applicable stabilized-approach gate in `737-approach`, with required visual references, verified landing performance, and actual manual control. Merely announcing a manual landing does not satisfy these conditions. Do not claim an unavailable LAND annunciation.
4. Keep checking IAS, pitch/bank trends, altitude/height, vertical speed, receiver validity/deviations, CMD status, and active/armed modes through minima and flare. Do not repair a late ILS failure with heading, V/S, LVL CHG, or route modes. Continue below the applicable decision point only when the required landing conditions are satisfied; otherwise use `737-go-around`.
5. If an authorized manual landing is planned, disconnect automation using the documented controls and verify actual manual authority before handoff. Use the documented visual-reference, flare, and thrust procedure; do not wait for automatic flare on a single-channel approach.

## Preserve monitoring time on low final

- Do not assume a fixed amount of flight time per tool call. Use fresh height, vertical speed, IAS, and their trends to judge the remaining margin; at a steady descent, height divided by sink rate gives only an approximate time to ground, not a flare trigger.
- On low final, alternate focused instrument reads and necessary control corrections, aiming for 1–2 second feedback as latency permits. Never batch unrelated catalog calls or other tasks to consume time toward flare: the aircraft descends while those calls run. If the available feedback or control authority cannot support a safe landing, go around while there is margin rather than waiting for a last-second disconnect.

## Touch down and stop

- Observe the expected flare and thrust reduction, runway alignment, actual touchdown, and on-ground indication. Do not claim a landing from a low altitude or mode label alone. If the approach becomes unsafe before touchdown, go around.
- After touchdown, verify speedbrake deployment and braking/deceleration. Use the documented reverse-thrust procedure and return reversers to idle/stowed at its specified speed. If autobrake does not decelerate the aircraft, use supported manual braking and verify its response. Maintain directional control and monitor remaining landing distance.
- Continue until stopped as required by the scenario. Do not retract landing configuration during high-speed rollout. Once slow and clear of the runway when authorized, execute and record the actual after-landing section: verify prescribed flap/speedbrake, start-switch, lights, transponder, and other states from its live items. Select autobrake by the catalog's labeled detents: a zero value can select RTO, not OFF. Compare `detail` and the mapped `autobrake-position` reading with OFF before marking; correct a mismatched detent rather than calling RTO off.

## Close out warnings after cleanup

1. After all after-landing switch changes, independently verify on-ground state, near-zero groundspeed, and destination position. Obtain fresh `get_function_states` and `read_group` for `fire-and-emergency`; explicitly inspect both `master-caution-captain` and `master-caution-first-officer` states, system annunciations, and warning indications. Do not filter the function-state response to WXR or autoflight controls alone: a master-caution `on: true` remains an open caution even when the aircraft is stopped and the checklist is complete.
2. Identify each illuminated system's cause from its detailed readings and documented procedure before any acknowledgement/reset. Probe-heat OFF can produce pitot-off indications during after-landing cleanup; distinguish a prescribed ground configuration from an actual fault. Preserve the required switch configuration, use only the documented acknowledgement/reset after interpreting the indication, and never switch heat back on, inhibit a warning, or repeatedly reset merely to extinguish a lamp.
3. Re-read both master-caution states and the affected system/warning indications after any action and again after remaining switch changes. An acknowledgement does not repair a fault; check for persistence or recurrence. Do not declare warnings clear with either master caution on or with an unexplained indication. Report unresolved or unavailable indications explicitly rather than claiming a clear cockpit; silence and checklist acceptance are not clearance evidence.
