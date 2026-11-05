---
name: 737-go-around
description: Use when approach capture or stabilized landing conditions fail, or when a Boeing 737 must discontinue descent and fly the missed approach.
---

# Boeing 737 go-around and missed approach

## Prepare before approach

- Read the supported go-around controls/procedure and the selected chart's missed-approach track, altitude, climb gradient, turn restrictions and configuration schedule before intercept. Discover TO/GA, thrust and autopilot-disconnect controls early; do not search for them with terrain approaching.
- Go around at failed capture, the failed stabilized gate, lost guidance, missing required autoland modes, or minimums without the required references. Begin before terrain clearance is exhausted; neither changing heading/selected altitude nor setting V/S to zero is a go-around.

## Establish the climb first

1. Execute the documented TO/GA action and promptly verify both engines' thrust increase, go-around FMA and actual pitch response. If automation does not establish the safe flight path, use the documented disconnect/manual-recovery branch, set the required thrust and arrest descent with bounded pitch corrections. Do not wait for an issue report or keep pressing mode buttons while descending.
2. Follow valid go-around flight-director guidance and the weight/configuration-dependent target speed. For manual recovery under the documented procedure, smoothly aim toward the normal initial go-around attitude, approximately 15° nose up, adjusting for IAS and terrain clearance. Ease the sustained pitch input as the attitude approaches target and read its trend immediately; do not trade a low-speed margin for a high climb rate.
3. Select the prescribed initial go-around flap setting, normally flaps 15 from a normal landing configuration. Confirm rising altitude and positive vertical speed before gear UP, then verify retraction while continuing to monitor pitch, IAS and climb. Do not retract to clean configuration immediately at low height.
4. Establish the published missed-approach track and altitude, observing turn restrictions. An MCP altitude above the aircraft with active negative V/S does not command a climb; require verified climb modes, thrust and actual positive vertical speed. V/S zero may only arrest descent after a delay and provides no climb performance.
5. During recovery, alternate corrections with focused flight-deck reads as close to 1–2 seconds apart as latency permits, without deliberate waits. Read height AGL and its trend as well as altitude: terrain can rise faster than the aircraft. Do not perform a low-level repositioning turn or continue descending to regain the localizer.
6. Once a safe climb is established, use `737-climb` for the prescribed acceleration/flap schedule and `737-altitude-hold` for verified level-off at the missed-approach altitude. Report failed controls, then resolve blocked preparation and checklist items in stable flight before considering another approach. Do not try another approach unless its required data and safe intercept can be established.
