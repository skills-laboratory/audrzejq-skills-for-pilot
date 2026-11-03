---
name: 737-climb
description: Use after liftoff for stable climb, scheduled flap retraction, low-speed recovery, and verified autoflight handoff.
---

# Boeing 737 climb

## Stabilize before secondary tasks

- Maintain the departure track and procedure's initial climb speed with appropriate thrust and small pitch corrections. IAS falling with rising pitch calls for reduced pitch, not a larger sustained nose-up input to chase vertical speed.
- If IAS approaches the configuration's minimum maneuver speed or falls below the initial climb target, immediately unload by smoothly reducing pitch, keep wings approximately level, and apply appropriate available thrust. Disconnect automation if it impedes recovery. Do not retract more flaps, start a turn, search documents, or engage autopilot while speed/attitude is unsafe.
- Choose a modest recovery attitude appropriate to IAS and configuration. Use small corrections and immediate complete `flight-instruments` scans; budget for actual model/command delay as in `boeing-737-pilot`. Release nose-down input before the projected attitude passes the recovery target, not after vertical speed turns negative. Keep scanning after neutralization: counter continued pitch drift, stabilize, then trim persistent holding force and verify the response. If descent has begun, smoothly arrest it and return to a modest climb. A stall warning requires the applicable recovery procedure without waiting for checklist work.
- Recovery is not complete because the control ratio is zero or IAS has improved once. Require successive scans showing safe IAS without a deteriorating trend, arrested pitch motion, and positive climb before gear verification, flap changes, mode selections, or checklist marks. If the assigned altitude is approaching, prioritize controlled capture instead of further cleanup.

## Accelerate and clean up

- Above 400 ft using the procedure's stated altitude datum, select or verify the permitted roll mode. Use LNAV only with a valid active route and confirmed FMA; otherwise use the documented departure roll-mode branch.
- At the assigned acceleration/retraction conditions, establish a stable accelerating climb using the bounded corrections above. Retract flaps one scheduled detent at a time using the weight-dependent FMC/PFD maneuver-speed schedule, only while the stability gate remains satisfied. After each selection, scan pitch/rate, IAS/trend, and vertical speed before verifying actual flap/slat movement or making another selection. If pitch runs away or IAS deteriorates, suspend retraction and recover; do not combine a recovery pitch command with the next flap command. Height alone is not permission to retract.
- After actual flap/slat retraction, execute the remaining takeoff checks: prescribed VNAV mode, autopilot as needed, engine start switches as required, autobrake OFF, and gear lever OFF. Keep the assigned MCP altitude limit in place and mark only verified items.

## Verify the autoflight handoff

1. With stable attitude, adequate airspeed, and procedure prerequisites satisfied, establish the documented pitch, roll, and thrust modes. Confirm actual FMA annunciations and targets before relying on them; a flight director does not move the aircraft, and autothrottle ARM does not control speed.
2. Engage the permitted autopilot channel when appropriate. Verify CMD, active pitch/roll modes, safe speed target, altitude target, and the aircraft's continuing response. Manage sustained manual inputs/overrides according to the documented handoff procedure; do not assume CMD alone has taken control.
3. Read targets again after every mode activation: a mode may synchronize speed or vertical speed to the current flight state. Restore the intended targets with the supported controls and verify them. Never retain a captured low speed or negative vertical speed for an intended climb.
4. If using V/S under a permitted procedure branch, verify its sign and magnitude after activation and after setting it, as well as actual vertical speed. If the setter reports a different value, treat it as unresolved even when `verified` is true. Do not increase climb rate at the expense of safe IAS.
5. A blank/wrong FMA, unverified selection, or continuing descent means the handoff is not complete. Maintain or regain manual control, report inconsistent tool behavior, and resolve the documented prerequisites rather than repeatedly toggling modes. Load `737-altitude-hold` before altitude capture.
