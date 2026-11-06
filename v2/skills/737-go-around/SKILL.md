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

1. Use the briefed aircraft go-around procedure and the chart's missed-approach track, altitude, gradients and turn limits. Apply TO/GA as prescribed and verify throttle movement and both engines' response; autothrottle ARM or an N1 annunciation alone does not establish go-around thrust. If automatic thrust is absent, use the documented manual thrust control while maintaining attitude and safe IAS.
2. Immediately read CMD A/B and actual pitch/roll modes. A TO/GA flight-director mode with both CMD channels OFF is guidance, not automatic pitch control. Use the documented manual-control procedure and brief, bounded corrections to fly the valid guidance; do not wait for a roll mode or engine spool-up to raise the nose. For a normal go-around, initial pitch is typically about 15° nose up, adjusted to the aircraft procedure, IAS and valid guidance; an upset or stall requires the recovery above instead.
3. Select and verify the prescribed go-around flap detent, normally flaps 15 from a flaps 30/40 approach, and stow the speedbrake. Read IAS, attitude and flight-path trends immediately. Keep the published initial track; confirm rising altitude and positive vertical speed before gear UP, then verify retraction.
4. Read back the published missed-approach altitude on the MCP at the prescribed condition; do not retain an earlier descent/intercept target. Above the published acceleration conditions, accelerate, retract flaps on the maneuver-speed schedule and transition to the cleared climb/level-off. Verify control authority, active modes and the actual path before relying on automation; use `737-climb` and `737-altitude-hold` as applicable.
5. Continue control/readback through a verified climb and protected level-off; pressing TO/GA is not completion. Read and record the live go-around checklist at the next stable opportunity. For a landing goal, resume approach preparation and reattempt only after landing prerequisites and a safe, authorized intercept are established. A missing tool remains a reported limitation, not a completed action or justification for continuing an unsafe approach.
