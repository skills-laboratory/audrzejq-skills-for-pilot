---
name: 737-landing
description: Use after a stabilized Boeing 737 approach to verify autoland or manual landing, control rollout, and complete after-landing checks.
---

# Boeing 737 landing and stopping

## Verify the landing method before descending further

- Read the applicable landing-continuation documentation before final approach. Maintain the stabilized gates in `737-approach` and keep `737-go-around` available. A single CMD channel with APP armed does not establish autoland.
- For the documented dual-channel ILS, with the first channel flying active VOR/LOC and G/S, engage the second using the documented hold action, not a short channel-switching press. Do this promptly after capture, while still above approximately 1,500 ft height AGL. Read both CMD states, active VOR/LOC and G/S, and armed FLARE/ROLLOUT. Use only exposed indications; do not claim an unavailable LAND 3 annunciation.
- If a channel drops, required guidance is lost, or FLARE is not armed by 350 ft, discontinue autoland and go around. Do not repeatedly press CMD buttons at low altitude. A manual landing is a separate documented branch requiring verified runway references, safe autopilot/autothrottle handoff and a stable approach; it is not a last-second substitute for failed autoland.

## Touchdown and rollout

1. Monitor runway alignment, speed, sink rate, height and modes continuously without long wait/read batches. On autoland, verify the documented transition to active FLARE and ROLLOUT and actual thrust reduction. If it does not occur, act under the landing-continuation/go-around procedure rather than letting a fixed V/S command reach the ground.
2. For a documented manual landing, maintain the verified landing speed and centerline. Begin a gentle flare around 30–50 ft using small pitch changes to reduce sink, easing thrust as prescribed. Account for tool latency and actual height trend; a yoke ratio is not a pitch command. Avoid a large pitch input, floating, or trying to force touchdown from excessive sink or misalignment.
3. Verify actual runway touchdown and ground state before reverse thrust or ground braking. Confirm speedbrake deployment and the planned autobrake/deceleration; use documented manual braking if required. Maintain centerline with small directional corrections and manage reverse thrust and autopilot disconnect according to the rollout procedure. Keep flaps and landing braking configured until rollout is complete.
4. Confirm stopped ground speed, runway location, intact gear, idle thrust and current warnings before claiming a successful landing. Autopilot disconnect does not disconnect autothrottle: use the documented thrust/autothrottle handoff and verify both engines remain at idle when stopping. Ground contact without verified down-and-safe gear, or an off-runway stop, is an abnormal outcome; secure the aircraft under the applicable procedure, report it and do not attempt a restart. Do not claim a flare, gear extension or dual-channel engagement without the corresponding action and live evidence.

## After landing

- Enter routine after-landing cleanup only after verified runway touchdown, safe rollout and the documented after-landing point, not merely `on-ground` or zero speed after abnormal contact. Read/activate the live section. Select and verify autobrake OFF, speedbrake DOWN, prescribed probe heat and engine-start switches OFF, exterior lights as needed, weather radar OFF, flaps UP and the required transponder mode. Verify radar operating mode separately from its display overlay.
- Mark each completed item with `737-checklist` and read back progress. Do not perform these actions while airborne or during a go-around, and do not infer completed after-landing checks from impact-induced switch or gear states.
