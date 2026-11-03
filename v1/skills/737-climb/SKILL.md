---
name: 737-climb
description: Use after liftoff for stable climb, scheduled flap retraction, low-speed recovery, and verified autoflight handoff.
---

# Boeing 737 climb

## Stabilize before secondary tasks

- Maintain the departure track and procedure's initial climb speed with appropriate thrust and small pitch corrections. If above the intended attitude and still pitching up, set `pitch-control` to neutral (0), read immediately, and use a brief, small nose-down correction if the rise continues; merely reducing a positive ratio still commands back-pressure. Reassess pitch rate after a thrust or IAS increase instead of reusing a large ground/low-speed input. IAS falling with rising pitch calls for reduced pitch, not a larger sustained nose-up input to chase vertical speed.
- If IAS approaches the configuration's minimum maneuver speed or falls below the initial climb target, immediately unload by smoothly reducing pitch, keep wings approximately level, and apply appropriate available thrust. A high vertical speed alone is not a reason to reduce thrust while IAS is low and falling: reduce the excessive pitch instead. Disconnect automation if it impedes recovery. Do not retract more flaps, start a turn, search documents, or engage autopilot while speed/attitude is unsafe.
- Choose a modest recovery attitude appropriate to IAS and configuration, then use bounded pitch corrections with immediate reads of IAS, pitch trend, vertical speed, and height AGL, aiming for 1–2 second feedback without deliberate waits. Estimate time to that attitude from remaining degrees and observed pitch rate, including reading, decision, and control-call delay. Remove the sustained nose-down input before the next cycle would pass the attitude; a smaller negative ratio still lowers the nose, and neutral does not instantly arrest pitch motion. Use brief, small counter-corrections as needed to stop the trend, while preserving safe IAS; do not wait for negative vertical speed. Confirm successive reads show safe IAS, arrested pitch trend, and positive climb before secondary tasks. If descent has begun, smoothly arrest it and return to a modest climb. A stall warning requires the applicable recovery procedure without waiting for checklist work.

## Accelerate and clean up

- Above 400 ft using the procedure's stated altitude datum, select or verify the permitted roll mode. Use LNAV only with a valid active route and confirmed FMA; otherwise use the documented departure roll-mode branch.
- At the assigned acceleration/retraction conditions, lower pitch enough to accelerate using the bounded corrections above, then remove the nose-down correction and verify the new attitude is holding before cleanup. After any nose-up correction, likewise arrest rising pitch before a flap or mode call; a smaller positive ratio is not a stabilized climb. Retract flaps one scheduled detent at a time using the weight-dependent FMC/PFD maneuver-speed schedule. Verify actual flap/slat movement and recheck pitch trend, IAS, and positive climb after each selection before the next secondary task. Do not use height alone or a falling IAS as permission to retract.
- After actual flap/slat retraction, execute the remaining takeoff checks: prescribed VNAV mode, autopilot as needed, engine start switches as required, autobrake OFF, and gear lever OFF. Keep the assigned MCP altitude limit in place and mark only verified items.

## Verify the autoflight handoff

1. Start mode setup only after successive instrument reads show adequate IAS, the intended attitude, an arrested pitch trend, and positive climb, with procedure prerequisites satisfied. Establish the documented pitch, roll, and thrust modes. If pitch starts running away or IAS becomes unsafe during the sequence, interrupt mode work and recover before another button press. Confirm actual FMA annunciations and targets before relying on them; a flight director does not move the aircraft, and autothrottle ARM does not control speed.
2. Engage the permitted autopilot channel when appropriate. Verify CMD, active pitch/roll modes, safe speed target, altitude target, and the aircraft's continuing response. Manage sustained manual inputs/overrides according to the documented handoff procedure; do not assume CMD alone has taken control.
3. Read targets again after every mode activation: a mode may synchronize speed or vertical speed to the current flight state. Restore the intended targets with the supported controls and verify them. Never retain a captured low speed or negative vertical speed for an intended climb.
4. If using V/S under a permitted procedure branch, verify its sign and magnitude after activation and after setting it, as well as actual vertical speed. If the setter reports a different value, treat it as unresolved even when `verified` is true. Do not increase climb rate at the expense of safe IAS.
5. A blank/wrong FMA, unverified selection, or continuing descent means the handoff is not complete. Maintain or regain manual control, report inconsistent tool behavior, and resolve the documented prerequisites rather than repeatedly toggling modes. Load `737-altitude-hold` before altitude capture.
