---
name: 737-descent
description: Use for an airborne arrival or before descent to brief the approach, obtain landing performance and maintain a safe intercept path.
---

# Boeing 737 descent and arrival preparation

## Stabilize and brief

1. Read actual IAS, altitude, height AGL, pitch, bank, vertical speed, CMD and active FMA modes. Verify the assigned safe altitude, heading and speed before working on the FMC or checklists; the loaded scenario description is not a current instrument reading. Keep functioning automation coupled during preparation and interleave focused instrument reads with setup calls.
2. Read the selected arrival/approach chart, current aircraft approach procedure and landing continuation. Establish runway and threshold elevation, navigation identifiers, distance reference, protected altitudes, intercept, minima and missed approach. Load `737-ils-approach`, `737-landing` and `737-go-around` before their actions become urgent.
3. Distinguish ILS DME, VOR DME and distance to the threshold. Compare a chart altitude only with the distance source named by that chart; do not apply a VOR-distance table to an ILS receiver. A rough 3° geometric check is threshold elevation plus threshold crossing height plus about 320 ft per NM to the threshold. It is not clearance to descend below published or assigned altitudes. Verify the documented glide-slope needle sense and signal validity rather than inferring above/below from a full-scale number alone.

## Prepare and record

- Use `737-checklist` for the live descent and approach categories. Verify selected pressurization landing altitude, system-annunciator recall, navigation radios/courses, applicable minimums, autobrake, lights and other conditional items independently, then mark each supported item. A broken VREF entry does not justify leaving verified radio or autobrake items unrecorded.
- Obtain landing flap setting and weight-dependent VREF from valid aircraft performance data; apply the documented speed correction. Read the APPROACH REF labels, enter at the supported field and verify accepted flap/speed data outside the scratchpad. Blank gross weight or dashed VREF is missing performance data, not permission to invent a fixed landing speed. Report the limitation and use a documented alternative only if available; otherwise retain a safe maneuvering speed and arrange a protected hold or missed approach rather than committing to final.
- Obtain the applicable QNH and use the chart minima row appropriate to the available pressure source. Do not assume 29.92 is local QNH or convert a threshold-relative chart height directly to a terrain-relative radio setting; use the specified barometric/radio datum and never round minimums down.

## Establish the intercept

- Plan deceleration and flap extension using the actual weight/configuration maneuver speeds and placard limits. Select a chart/clearance-supported intercept altitude and verify capture below the glide slope; do not choose an arbitrary lower MCP altitude to chase the beam.
- In level change, read the active pitch/thrust modes and recheck selected speed/altitude and actual trends. If a mode call reports no change, verify whether it is already active. Allow for the observed deceleration response while monitoring terrain clearance; use only a documented alternative if the expected response remains absent.
- If setup cannot finish before intercept, or the aircraft cannot reach a safe intercept from below, extend or hold only within the cleared protected procedure, or go around. Do not disconnect working automation and dive to catch the approach. Continue with `737-ils-approach` once the intercept and essential landing data are verified.
