---
name: 737-climb
description: Use after liftoff for stable climb, scheduled flap retraction, low-speed recovery, and verified autoflight handoff.
---

# Boeing 737 climb

## Stabilize before secondary tasks

- Maintain the departure track and procedure's initial climb speed with appropriate thrust and small pitch corrections. IAS falling with rising pitch calls for reduced pitch, not a larger sustained nose-up input to chase vertical speed.
- If IAS approaches the configuration's minimum maneuver speed or falls below the initial climb target, immediately unload by smoothly reducing pitch, keep wings approximately level, and apply appropriate available thrust. Disconnect automation if it impedes recovery. Do not retract more flaps, start a turn, search documents, or engage autopilot while speed/attitude is unsafe.
- Choose a modest recovery attitude appropriate to IAS and configuration, then use bounded pitch corrections with immediate reads of IAS, pitch trend, vertical speed, and height AGL, aiming for 1–2 second feedback without deliberate waits. Estimate time to that attitude from remaining degrees and observed pitch rate, including reading, decision, and control-call delay. Remove the sustained nose-down input before the next cycle would pass the attitude; a smaller negative ratio still lowers the nose, and neutral does not instantly arrest pitch motion. Use brief, small counter-corrections as needed to stop the trend, while preserving safe IAS; do not wait for negative vertical speed. Confirm successive reads show safe IAS, arrested pitch trend, and positive climb before secondary tasks. If descent has begun, smoothly arrest it and return to a modest climb. A stall warning requires the applicable recovery procedure without waiting for checklist work.

## Accelerate and clean up

- Above 400 ft using the procedure's stated altitude datum, select or verify the permitted roll mode. Use LNAV only with a valid active route and confirmed FMA; otherwise use the documented departure roll-mode branch.
- At the assigned acceleration/retraction conditions, lower pitch enough to accelerate using the bounded corrections above, then remove the nose-down correction and verify the new attitude is holding before cleanup. After any nose-up correction, likewise arrest rising pitch before a flap or mode call; a smaller positive ratio is not a stabilized climb. Retract flaps one scheduled detent at a time using the weight-dependent FMC/PFD maneuver-speed schedule. Verify actual flap/slat movement and recheck pitch trend, IAS, and positive climb after each selection before the next secondary task. Do not use height alone or a falling IAS as permission to retract.
- After actual flap/slat retraction, execute the remaining takeoff checks: prescribed VNAV mode, autopilot as needed, engine start switches as required, autobrake OFF, and gear lever OFF. Keep the assigned MCP altitude limit in place and mark only verified items.

## Verify the autoflight handoff

1. With stable attitude, adequate airspeed, and procedure prerequisites satisfied, establish the documented pitch, roll, and thrust modes. Confirm actual FMA annunciations and targets before relying on them; a flight director does not move the aircraft, and autothrottle ARM does not control speed.
2. Engage the permitted autopilot channel when appropriate. Verify CMD, active pitch/roll modes, safe speed target, altitude target, and the aircraft's continuing response. Manage sustained manual inputs/overrides according to the documented handoff procedure; do not assume CMD alone has taken control. For a manual takeover, use the documented disconnect and read both CMD channels to verify disengagement; do not stack sustained manual pitch commands on an engaged autopilot. Keep the flight-instrument feedback loop running throughout the handoff or recovery.
3. Read targets again after every mode activation: a mode may synchronize speed or vertical speed to the current flight state. Restore the intended targets with the supported controls and verify them. Never retain a captured low speed or negative vertical speed for an intended climb.
4. If using V/S under a permitted procedure branch, verify the active V/S FMA, then set and read back the intended sign and magnitude, as well as actual vertical speed. If activation synchronized the target, restore it once and verify. A setter reporting a different value remains unresolved even when `verified` is true; if the mismatch persists, report it and use a verified alternate mode or manual flight, not repeated setter calls. Do not increase climb rate at the expense of safe IAS.
5. After a no-change or unverified mode call, read the live FMA, channel state, and targets before another press: the mode may have activated despite the tool response. A blank/wrong FMA or continuing descent means the handoff is not complete. Maintain or regain manual control and report inconsistent tool behavior; defer further mode troubleshooting until attitude and IAS are stable and the documented prerequisites are resolved. Load `737-altitude-hold` before altitude capture.
