---
name: 737-approach
description: Use after arrival preparation for a verified ILS intercept, configuration, glide-slope capture, and stabilized final approach.
---

# Boeing 737 ILS approach

## Intercept without chasing an unverified beam

1. Confirm the assigned runway/procedure, receiver identifiers and courses, QNH/minima, distance reference, safe intercept altitude, and landing speeds from `737-arrival`. Establish a suitable localizer intercept, preferably within 30 degrees, with the glide slope above the aircraft. Maintain the cleared, terrain-safe intercept altitude until capture; do not start a continuous V/S descent merely because APP is armed.
2. Arm APP once and read active and armed FMA indications. Armed VOR/LOC and G/S are not capture. Require active VOR/LOC with valid, converging lateral guidance for localizer capture, then active G/S with valid vertical guidance and actual steady descent for glide-slope capture. Resolve an unverified tool response with these readings, not repeated APP presses.
3. Cross-check the chart's glidepath altitude at the actual distance from its named aid. Do not guess the sign of a numeric needle: use documented conventions and displayed guidance. A valid signal flag with a pegged or contradictory deviation does not establish glide slope alive or authorize descent. If the guidance cannot be reconciled, maintain a safe altitude while there is room; discontinue the approach and use `737-go-around` if capture cannot be established safely. Do not salvage it by diving from above or inventing a localizer-only clearance/minima.

## Configure at the observed conditions

- Schedule initial flaps and deceleration using the weight-dependent maneuver speeds and flap limits. Verify actual IAS, flap/slat movement, and flight path after each selection. If IAS remains high despite the selected speed, resolve thrust/drag and approach geometry before continuing; do not assume the MCP has achieved the target.
- At verified glide slope alive, execute the documented ILS sequence: gear DOWN and three independent green indications, flaps 15, both engine start switches CONT, speedbrake ARM and the distinct ARMED annunciator. Verify selector units/detents and actual indications. Interleave instrument reads and mark the corresponding live landing-section items as conditions occur.
- At verified G/S capture, select and verify the approved landing flap setting and approach speed. Set the charted missed-approach altitude at the procedure's capture condition, then immediately recheck that G/S remains active and the aircraft still descends. A higher selected altitude is not safe approach guidance if G/S is lost.
- For autoland, proceed immediately to the channel and armed-mode checks in `737-landing` while there is still adequate height. Never treat a single-channel ILS as an autoland.
- By the applicable stabilized-approach gate, require the correct landing configuration, safe planned IAS, appropriate thrust, and stable lateral/vertical path. Unless the procedure is stricter, use 1,000 ft above airport elevation in instrument conditions or 500 ft in visual conditions. If these conditions are not met, go around; do not substitute terrain AGL for airport-relative height.
