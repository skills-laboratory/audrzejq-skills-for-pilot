---
name: 737-ils-approach
description: Use before ILS intercept through final approach to verify capture, landing configuration, dual-channel readiness and stabilized flight.
---

# Boeing 737 ILS approach

## Intercept and capture

1. Complete the essential preparation in `737-descent`. Tune and identify both ILS receivers, verify both inbound courses, signal validity, the chart distance reference and minimums. Read the live approach and ILS checklist sections. Maintain a safe intercept altitude below the glide slope and a suitable heading, preferably within 30° of the localizer course.
2. With the permitted autopilot coupled, arm APP once and read active/armed FMA modes. VOR/LOC and G/S armed, VOR/LOC active, and G/S active are different conditions. Verify localizer capture, then glide-slope capture and the actual descent; a centered localizer needle, APP light or CMD light alone proves none of these.
3. For a no-change or unverified APP call, inspect current armed/active modes and documented prerequisites rather than toggling APP repeatedly. If capture fails, retain a safe flight path and use the protected missed approach. Do not force capture from above or use large manual roll/pitch inputs to repair it near the runway.

## Configure and verify

- Extend flaps by the weight-dependent maneuver-speed schedule and within placard limits, checking actual movement and IAS after each selection. At the conditions stated by the live ILS procedure, select gear down, required engine-start switch positions and speedbrake ARM; verify all gear down and the actual armed state, not only lever commands.
- After G/S capture, complete the specified landing flap selection and select the verified VREF plus documented correction. Once steady coupled descent is confirmed, set the published missed-approach altitude at the checklist condition and recheck G/S remains active; loss of G/S with a higher selected altitude can initiate a climb.
- If using the documented simulator autoland, engage the second channel with `cmd-b-hold` when CMD A is flying the coupled ILS, or `cmd-a-hold` for the opposite channel. The documented default hold is three seconds; a short CMD press changes channels, not dual-channel operation. Do this promptly while above about 1,500 ft height AGL, not near the documented 800 ft engagement lockout. Height AGL over terrain is not itself a radio-altimeter annunciation.
- Verify both CMD channels, VOR/LOC and G/S active, and FLARE and ROLLOUT armed at the documented heights. Do not claim an unavailable LAND 3 indication. If FLARE has not armed by 350 ft or a channel drops, go around rather than attempting repeated late CMD selections.

## Stabilized final

- Monitor IAS and trend, flight-path deviations, pitch/bank, vertical speed, height/altitude, thrust, gear/flaps and FMA between secondary tasks. Confirm the landing checklist is complete with actual evidence.
- Diagnose suspected tracking failure from valid G/S deviation magnitude and trend, active modes and successive flight-path reads together. For altitude cross-checks, use the chart's named distance source and the correct pressure datum as in `737-descent`; a high sink rate alone does not quantify how far above or below the beam the aircraft is. A steady 3° descent is roughly five times groundspeed in knots, expressed in ft/min, but configuration and deceleration can produce transients.
- Above the stabilization gate, idle thrust while IAS remains above the selected approach speed can be commanded deceleration, not autothrottle failure. Check whether speed and path converge without unnecessary mode changes. Unsafe or diverging flight, warnings, or inability to meet the stabilized criteria require a go-around; do not delay it to finish a diagnosis or checklist.
- Use the published stabilized-approach criteria; absent stricter criteria, require stability by 1,000 ft above aerodrome in instrument conditions or 500 ft in visual conditions: correct landing configuration, on path, speed between VREF and VREF plus 20 kt, appropriate thrust and normally no more than 1,000 ft/min descent unless specifically briefed. A stricter planned speed target still applies. Go around if these conditions are not met or cannot be maintained.
- At the applicable minimums, continue only with the required visual references or explicitly authorized autoland conditions. Do not substitute autoland capability for authorization to continue below minima. Use `737-landing` for flare and rollout, or `737-go-around` immediately when continuation is unsafe.
