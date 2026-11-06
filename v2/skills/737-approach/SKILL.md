---
name: 737-approach
description: Use for Boeing 737 ILS intercept, verified localizer and glide-slope capture, and landing configuration.
---

# Boeing 737 ILS approach

## Intercept and capture

1. Complete `737-descent` preparation and load the live landing sections. Verify valid ILS signals and identifiers, both receiver courses, active autopilot channel, flight directors, thrust mode, speed, and chart/clearance altitude constraints. Determine whether the glide slope is above or below the aircraft using the documented indication convention, not a guessed signed-dot interpretation.
2. Establish a suitable intercept heading, preferably within 30° of the localizer course, at an authorized altitude with the glide slope above the aircraft. A heading equal to the runway course merely flies parallel when offset. After the heading change, compare focused localizer reads as the turn settles; use the documented deviation convention and observed convergence, not the sign alone. If deviation grows or the aircraft crosses the centerline without capture, revise the intercept promptly rather than leave a fixed intercept heading while doing CDU work. Do not descend below segment limits to repair a localizer error.
3. Arm APP once using `cockpit_mcp_and_autopilot`, action `app`, and read the FMA. With HDG SEL/ALT HOLD active, no VOR/LOC or G/S in the armed fields means the ILS is not armed; V/S armed is not G/S armed. Valid receiver identifiers and populated performance data do not establish arming. Distinguish VOR/LOC and G/S armed from active VOR/LOC roll and active G/S pitch. Stay in the focused flight-path loop until actual lateral convergence and then a steady glide-slope descent are verified; HDG SEL plus V/S is not a coupled ILS, even with valid needles. If a command reports no change, inspect existing modes before another press. Record arming and captures separately with `737-checklist`, then move directly to the next observed configuration condition.

## Configure at the stated conditions

- Extend flaps on the weight-dependent maneuver-speed schedule without exceeding placard limits. At the procedure's glide-slope-alive condition, select gear DOWN and verify three independent safe/green indications, flaps 15 and actual movement, both engine start switches CONT, and speedbrake ARM plus its distinct ARMED lamp. Keep flight-path reads interleaved with configuration and checklist marking.
- At verified G/S capture, select the directed landing flap and its accepted VREF-based approach speed. Set the chart's missed-approach altitude at the prescribed condition and immediately verify G/S remains active; a higher selected altitude is safe only while the intended approach pitch mode remains engaged.
- For the documented dual-channel autoland, engage the second channel promptly after coupled capture, while above approximately 1,500 ft AGL: use `cmd-b-hold` with CMD A already engaged, or `cmd-a-hold` with CMD B. A short CMD press changes channels rather than establishing dual operation. Verify both CMD lights, VOR/LOC, G/S, and FLARE/ROLLOUT arming around 1,500 ft; do not defer toward the documented 800 ft radio-altitude lockout. Terrain AGL is not a dedicated radio-altimeter indication.
- Check the applicable stabilized-approach gate, normally 1,000 ft in instrument conditions or 500 ft in visual conditions: correct path, landing configuration, accepted approach speed, appropriate thrust, and completed applicable checks. A modest localizer error well before this gate calls for timely intercept/capture, not abandoning the task. Failed capture, unstable final approach, loss of required guidance, or inadequate visual reference at minimums requires `737-go-around`, not a late dive, mode-button chase, or unbriefed manual landing.
- Continue with `737-landing` once stable; keep reading instruments and approach modes rather than ending after announcing the next action.
