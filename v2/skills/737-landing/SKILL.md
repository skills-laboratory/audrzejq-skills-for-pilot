---
name: 737-landing
description: Use after verified ILS capture to monitor Boeing 737-800 landing configuration, dual-channel autoland where authorized, touchdown, rollout, and stopping.
---

# Boeing 737 ILS landing and stopping

## Verify the landing plan before final descent

- Continue from `737-approach` with the landing/after-landing sections and aircraft landing continuation available. Confirm the intended runway, valid ILS identification, active VOR/LOC and G/S, gear DOWN with three independent safe indications, actual landing flaps, corrected weight-dependent VREF target, required start switches, autobrake, and speedbrake ARMED indication.
- Keep checking IAS/trend, vertical speed, altitude, height, localizer/glide-slope deviations, FMA, and CMD channels between configuration/checklist calls. Mark only the applicable items supported by these observations using `737-checklist`; accepted marks do not prove capture, configuration, or touchdown.

## Verify dual-channel autoland when authorized

1. Use the installed aircraft's autoland procedure only when the scenario/approach authorizes it. One CMD channel following the ILS is not autoland. Complete the neutral-input/override handoff in `boeing-737-pilot` if returning from manual control.
2. With APP selected and the first CMD channel tracking the captured ILS, engage the second channel using the documented hold action once: `cmd-b-hold` when CMD A is flying, or `cmd-a-hold` when CMD B is flying. A short CMD press changes channels rather than establishing dual-channel operation.
3. Engage promptly while still above approximately 1,500 ft and verify both CMD channels, active VOR/LOC and G/S, and FLARE/ROLLOUT arming as required by the installed procedure. Height AGL is terrain clearance, not a dedicated radio-altimeter indication; use the procedure's stated datum and do not defer engagement toward its low-altitude lockout. Do not invent a LAND 3 indication when none is exposed.
4. If a channel drops, required modes fail, or FLARE is not armed by the procedure's 350 ft check, go around. Do not repeatedly press CMD or make a late manual landing an improvised substitute for failed autoland.

## Stable approach, touchdown, and rollout

- Be stable by the applicable gate, normally 1,000 ft in instrument conditions or 500 ft in visual conditions, unless the procedure is stricter: correct runway alignment/path, landing configuration complete, IAS close to the planned target, appropriate thrust, and a steady descent normally no more than 1,000 ft/min unless specifically briefed. Go around if these conditions cannot be maintained, or required visual references are absent at minimums.
- Use the charted altitude/height datum for minimums. Do not substitute terrain height AGL for barometric decision altitude or claim visual runway acquisition from coordinates or needle position alone.
- On a verified autoland, monitor FLARE, thrust reduction, runway alignment, and actual touchdown without adding manual pitch/roll inputs. If authorized manual landing is planned instead, follow the aircraft's manual flare procedure with small closed-loop corrections; never carry a sustained approach input into the flare unattended.
- Verify actual ground contact before reverse thrust: use on-ground/gear-load evidence and speed/vertical-path response, not a phase label or checklist completion. Monitor spoiler deployment, braking and directional control; use symmetrical reverse and its speed-dependent stow sequence from the aircraft procedure. Keep reversers stowed while airborne.
- Continue controlling rollout until actual groundspeed confirms the aircraft has stopped at the destination. Resolve remaining warnings through their causes, not by silencing or inhibiting them to claim a clear cockpit. Perform and record applicable after-landing cleanup when safely slowed/stopped, respecting runway-clear conditions. Report completion only from verified destination, touchdown, stopped state, and warning indications.
