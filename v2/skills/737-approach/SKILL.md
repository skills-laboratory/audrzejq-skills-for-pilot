---
name: 737-approach
description: Use during descent or an initialized airborne arrival to prepare and intercept the selected Boeing 737-800 ILS without losing runway geometry or capture conditions.
---

# Boeing 737 approach preparation and ILS intercept

## Prepare while the aircraft remains controlled

1. Load `737-checklist`, `737-landing`, and `737-go-around`. Read the current descent/approach sections, selected chart, aircraft ILS procedure, and missed approach while stable automation maintains a safe flight path. Do not disengage functioning CMD simply to begin preparation.
2. Read actual position, IAS/groundspeed, altitude/QNH, configuration, FMA, and selected targets. Establish the published inbound course, entry/intercept altitude, distance reference, runway threshold elevation, minimums, and missed-approach track/altitude. Distinguish chart DME, ILS DME, and distance to threshold; do not substitute one for another.
3. Check remaining distance after each setup block: minutes available are approximately distance in NM divided by groundspeed in kt, multiplied by 60. The aircraft keeps moving during CDU entries, searches, and checklist calls. If setup or a safe intercept cannot be completed in the remaining distance, use the published missed approach or an authorized safe reposition rather than pressing on toward the runway.
4. Verify landing altitude/pressurization, system recall, local altimeter setting, minimums, required lights/signs, navigation performance as applicable, and autobrake. Establish landing flaps and weight-dependent VREF from valid performance data, with the required speed correction. Read the accepted APPROACH REF selection, not merely the scratchpad; placeholders or INVALID ENTRY are unresolved. If data remains unavailable, report it and stabilize/reposition rather than inventing VREF or repeatedly typing while passing the intercept.
5. Tune both receivers to the charted ILS frequency and verify both identifiers and courses. Use supported reading identifiers from the current catalog. Select speeds compatible with the current flap configuration and its maneuver/extension limits; do not command final landing speed while still clean. Configure progressively and read actual flap/slat movement after each selection.

## Preserve the published approach geometry

- Verify that the aircraft is on the approach side of the intended threshold and will fly the published inbound course toward it. A bearing to the airport from the opposite side is not the inbound ILS course. Do not replace the published course with its reciprocal or attempt to use the same ILS for the opposite runway.
- Use charted fixes or verified runway coordinates for repositioning, with true/magnetic bearings distinguished. Do not infer a new localizer origin from guessed beacon coordinates. If navigation evidence conflicts with the chart, maintain safe altitude, report the discrepancy, and resolve it before descent on that guidance.
- A centered or zero localizer value with a missing identifier is not evidence of alignment. Require valid identification/signal indications, correct runway-side geometry, and appropriate active FMA before relying on guidance.

## Intercept from below and verify each transition

1. Establish a safe charted intercept altitude below the glidepath and a suitable heading, preferably within 30 degrees of the inbound course. Preserve altitude restrictions; do not dive from above close to the runway to chase the glide slope.
2. If using V/S before intercept, select the appropriate lower altitude and activate V/S, then read the FMA and set/read back the intended descent target in supported 100 ft/min increments. Mode activation can synchronize V/S; a setter reporting zero or another value does not establish the requested descent. Check actual altitude, IAS, and vertical-speed response before another adjustment.
3. Arm APP once and verify VOR/LOC and G/S armed separately. Localizer capture requires active VOR/LOC with valid, converging lateral guidance; APP illumination alone is insufficient. Glide slope alive requires valid vertical guidance moving toward capture, not a pegged value or a single zero reading.
4. At the procedure's glide-slope-alive condition, select gear DOWN and verify nose/left/right safe indications, flaps 15 with actual configuration, both engine start switches CONT, and speedbrake ARM with its distinct ARMED annunciator. Use documented detents, not an assumed percentage, and record verified applicable items with live checklist IDs.
5. Glide-slope capture requires active G/S, valid guidance, and a steady descending flight path. At capture, select the planned landing flaps within their limits, verify configuration and corrected VREF target, then set/read back the charted missed-approach altitude. Immediately recheck that G/S remains active: loss of G/S with a higher selected altitude can command a climb.
6. Continue with `737-landing`. If valid capture or a stable landing cannot be achieved, use `737-go-around`; do not repeatedly toggle APP or repair a late approach with heading/V/S/level-change modes.
