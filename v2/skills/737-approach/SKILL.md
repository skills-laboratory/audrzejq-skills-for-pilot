---
name: 737-approach
description: Use during descent or an initialized airborne arrival to prepare landing data, assess alerts, and verify ILS capture before final approach.
---

# Boeing 737 approach preparation and ILS capture

## Prepare while there is time

- Read actual position, altitude, IAS, vertical speed, configuration, active/armed FMA, selected targets, and alerts immediately. Preserve verified stable automation while preparing; an initial scenario description or phase label is not the current flight state. Interleave flight-instrument reads with documentation and checklist work.
- Read the assigned approach chart and aircraft landing, autoland, and missed-approach procedures using the available documentation tools. Brief runway, inbound course, intercept altitude, minima and their datum, missed-approach track/altitude, and landing distance. Keep each chart's DME station and threshold-distance reference distinct; do not apply one aid's profile altitudes to another receiver's distance.
- Verify local QNH against the actual altimeter settings. Tune and identify both ILS receivers and set both courses. Set the applicable minimums and seek an actual read-back; an unavailable minimums indication remains unverified, not confirmed by a successful setter.
- Obtain landing weight and the chosen flap setting's VREF from APPROACH REF. If weight or VREF is blank, read current gross weight and fuel and initialize the necessary FMC performance fields in their displayed units. For thousands of pounds from kilogram readings, ZFW = (gross weight - fuel) × 2.2046 / 1000. Verify the resulting FMC gross weight and landing reference; do not copy example weights or infer acceptance from scratchpad text. Set and verify VREF plus the applicable procedure/wind correction on the MCP.
- Finish applicable descent/approach checks before intercept when possible. Conditional items require their actual trigger; temporary flaps 15 does not call for a flaps-15 landing inhibit. Report missing indication evidence rather than marking it to improve progress.

## Assess alerts before a busy final

- Read master caution/warning and the relevant system annunciators early. Identify the affected system, read the applicable non-normal procedure, and verify the individual fault indications before changing switches. For an air-conditioning caution, cross-check pack selectors, available pack/trip indications, bleed supply, duct pressure, and cabin altitude/rate; AUTO selectors and pressurized ducts alone do not prove the packs are operating.
- Do not cycle packs, bleeds, or unrelated systems experimentally, or reset an alert merely to obtain a clear indication. Use only the identified procedure's actions and recheck the underlying condition; acknowledgement is not fault correction. Keep flight-path reads between troubleshooting steps.
- If the interface cannot identify the fault, report the limitation and keep the condition unresolved. Establish whether the non-normal procedure permits landing and whether required systems remain available. If more assessment time is needed and prompt landing is not required, discontinue the approach using `737-go-around`; do not carry uncertain troubleshooting into low final. A caution alone is not an automatic go-around or proof that landing is prohibited.

## Capture without mode cycling

1. Establish the chart's permitted intercept altitude and a suitable heading, normally within 30° of the localizer course, with the glide slope above the aircraft. Complete preparation early enough to intercept from below rather than remaining level until a steep catch-up descent is needed.
2. Inspect actual active/armed FMA before pressing APP. Arm it once if needed; verify VOR/LOC and G/S arming separately from active VOR/LOC and G/S capture. A button feedback flag or an APP light is not the capture evidence.
3. If a permitted descent before capture uses V/S, first read the active pitch mode and selected V/S. If V/S is already active, do not press its toggle again. Otherwise select it once and verify the mode, then set the intended descent target and read the window and actual response. A setter returning zero or a different target is unresolved even with `verified: true`; determine whether altitude capture or another mode made V/S unavailable rather than repeatedly sending larger descent targets.
4. Once G/S is active, stop V/S commands and preserve coupled guidance. Verify centered/trending localizer and glide-slope deviations and actual descent. If the path cannot be safely established with room to stabilize, reposition or go around; do not dive for the glide slope close to the runway.
5. At observed glide slope alive, perform the prescribed gear DOWN/three-green, flap 15, both start switches CONT, and speedbrake ARM checks at safe configuration speeds. Verify actual states and the separate ARMED indication when available; lever selection does not substitute for a missing lamp. Continue with `737-landing` and record only evidenced items using `737-checklist`.
