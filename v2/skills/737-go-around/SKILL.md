---
name: 737-go-around
description: Use when an approach is unstable, capture or landing prerequisites fail, or a missed approach is required; recover attitude first if upset.
---

# Boeing 737 go-around and approach recovery

## Recover control first

- An upset is not a normal coupled go-around. Stop secondary tasks, read bank/pitch, IAS, vertical speed and terrain clearance, and disconnect automation if it impedes recovery. Use the documented manual-control/override procedure and the bounded corrections in `boeing-737-pilot`.
- For a nose-low, steep-bank upset, roll toward wings level before applying substantial nose-up recovery; pulling hard while steeply banked increases load without restoring the required vertical lift. Arrest growing roll with a brief opposite input, ease it before wings level and immediately read the response. Then smoothly arrest descent with pitch and thrust appropriate to IAS and height. Do not use trim as an immediate attitude control or assume CMD will recover an upset.
- If a stall warning or unsafe low speed occurs, reduce angle of attack, keep wings approximately level and apply appropriate available thrust before demanding a climb. Follow the applicable terrain-escape procedure if a terrain warning requires it. Do not retract flaps or attempt autopilot handoff while attitude or speed remains unsafe.

## Execute the missed approach

1. Use the already briefed aircraft go-around procedure and the missed-approach track, altitude, gradients and turn limits from the selected chart. Apply TO/GA as prescribed and verify engine response and actual pitch/roll/thrust modes; autothrottle ARM or a button press does not establish go-around thrust. Control manually if the coupled response is unavailable or unsafe.
2. Select the prescribed go-around flap detent and follow valid flight-director guidance with safe IAS and bounded pitch corrections. Confirm rising altitude and positive vertical speed before gear UP. Keep the published initial track; do not invent a low-altitude turn toward the runway.
3. Above the published acceleration conditions, accelerate, retract flaps on the maneuver-speed schedule and transition to the cleared climb/level-off. Verify each target, active mode and the actual path; use `737-climb` and `737-altitude-hold` as applicable.
4. Maintain control and read the live go-around checklist at the next stable opportunity. Reattempt only after landing prerequisites and a safe intercept are established. A missing tool remains a reported limitation, not a completed action or justification for continuing an unsafe approach.
