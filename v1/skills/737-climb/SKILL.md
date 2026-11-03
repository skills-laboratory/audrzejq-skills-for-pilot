---
name: 737-climb
description: Use after liftoff for stable climb, scheduled flap retraction, low-speed recovery, and verified autoflight handoff.
---

# Boeing 737 climb

## Stabilize before secondary tasks

- Maintain the departure track and procedure's initial climb speed with appropriate thrust and small pitch corrections. IAS falling with rising pitch calls for reduced pitch, not a larger sustained nose-up input to chase vertical speed.
- If IAS approaches the configuration's minimum maneuver speed or falls below the initial climb target, immediately unload by smoothly reducing pitch, keep wings approximately level, and apply appropriate available thrust. Disconnect automation if it impedes recovery. Do not retract more flaps, start a turn, search documents, or engage autopilot while speed/attitude is unsafe.
- Choose a modest recovery attitude appropriate to IAS and configuration. Immediately after each correction, read IAS, pitch rate, vertical speed, and height AGL; aim for 1–2 second feedback without deliberate waits. Project pitch through the measured full read-to-control delay as in `boeing-737-pilot`; neutralize the nose-down input before that projection passes the recovery attitude, rather than waiting for level pitch or descent. If IAS is safe and pitch is already rising toward a modest climb attitude, ease back-pressure before another read instead of adding more to chase a still-negative vertical speed. Use small counter-corrections if pitch rate persists through neutral. Confirm safe IAS, arrested pitch trend, and positive climb on successive reads before secondary tasks; smoothly arrest any descent. A stall warning requires the applicable recovery procedure without waiting for checklist work.

## Accelerate and clean up

- Above 400 ft using the procedure's stated altitude datum, select or verify the permitted roll mode. Use LNAV only with a valid active route and confirmed FMA; otherwise use the documented departure roll-mode branch.
- At the assigned acceleration/retraction conditions, lower pitch enough to accelerate using the bounded corrections above, then remove the nose-down correction and verify the new attitude is holding before cleanup. After any nose-up correction, likewise arrest rising pitch before a flap or mode call; a smaller positive ratio is not a stabilized climb. Retract flaps one scheduled detent at a time using the weight-dependent FMC/PFD maneuver-speed schedule. Verify actual flap/slat movement and recheck pitch trend, IAS, and positive climb after each selection before the next secondary task. Do not use height alone or a falling IAS as permission to retract.
- After actual flap/slat retraction, execute the remaining takeoff checks: prescribed VNAV mode, autopilot as needed, engine start switches as required, autobrake OFF, and gear lever OFF. Keep the assigned MCP altitude limit in place and mark only verified items.

## Verify the autoflight handoff

1. With stable attitude, adequate airspeed, and procedure prerequisites satisfied, establish the documented pitch, roll, and thrust modes. Confirm actual FMA annunciations and targets before relying on them; a flight director does not move the aircraft, and autothrottle ARM does not control speed.
2. Engage the permitted autopilot channel when appropriate. Verify CMD, active pitch/roll modes, safe speed target, altitude target, and the aircraft's continuing response. Manage sustained manual inputs/overrides according to the documented handoff procedure; do not assume CMD alone has taken control.
3. Read targets again after every mode activation: a mode may synchronize speed or vertical speed to the current flight state. Restore the intended targets with the supported controls and verify them. Never retain a captured low speed or negative vertical speed for an intended climb.
4. If using V/S under a permitted procedure branch, verify its sign and magnitude after activation and after setting it, as well as actual vertical speed. If the setter reports a different value, treat it as unresolved even when `verified` is true. Do not increase climb rate at the expense of safe IAS.
5. A blank/wrong FMA, unverified selection, or continuing descent means the handoff is not complete. Maintain or regain manual control, report inconsistent tool behavior, and resolve the documented prerequisites rather than repeatedly toggling modes. Load `737-altitude-hold` before altitude capture.
