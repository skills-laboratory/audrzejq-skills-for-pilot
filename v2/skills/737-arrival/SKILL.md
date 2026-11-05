---
name: 737-arrival
description: Use at the start of an airborne arrival or before descent to prepare landing performance, radios, minimums, and verified checklists.
---

# Boeing 737 arrival preparation

## Preserve control and brief the approach

1. Read actual position, altitude, IAS, configuration, CMD status, FMA, and selected targets. Preserve a functioning heading/altitude/speed hold while preparing. Recheck the instruments and distance to intercept between preparation tasks; the aircraft keeps moving during CDU work.
2. Use `search_docs` and `read_docs` for the assigned arrival, approach chart, aircraft procedures, landing continuation, and missed approach. Keep one selected procedure and its distance source together. VOR DME, ILS DME, and distance to threshold are not interchangeable; identify the tuned aid before using any distance/altitude table. Without an FMC route, use the documented conventional-navigation branch, not LNAV/VNAV.
3. Brief the intercept altitude, restrictions, landing configuration, minima, and missed-approach track/altitude. Charted glidepath check altitudes are cross-checks, not permission to descend below restrictions. Use QNH and the chart's barometric DA/MDA unless an explicit radio-altimeter setting is prescribed; a parenthesized height above threshold is not automatically a radio DH. If the minimums control cannot accept the barometric altitude, report the limitation and monitor the published DA/MDA against fresh QNH-corrected altitude readings; do not substitute radio DH merely to fit the knob's range.

## Complete preparation before intercept

- Verify selected pressurization LAND ALT, recall and interpret system annunciations, set applicable passenger signs/lights, verify altimeters and navigation performance, tune/identify the required receivers and courses, and set landing autobrake. Use the live descent and approach sections in `737-checklist`; mark each applicable verified item while still stable, then read section progress. Leave unobserved historical and unsatisfied conditional items unmarked.
- For system annunciations, inspect `fire-and-emergency` and its current control catalog: master-caution and six-pack actions are in this group. Do not declare annunciator controls absent because the flight-deck summary omits them or they are not in `tests-and-service`. Read the fault indications before resetting, follow the documented recall/reset procedure, and re-read the indications after resolving the cause. A reset is not proof of recall or fault clearance; report any genuinely missing required action or reading and leave that check unverified.
- Obtain landing weight and configuration-dependent VREF from approved aircraft performance data. Read the CDU title, labels, units, and scratchpad before entering data. Follow the documented gross-weight/ZFW entry path and any entry-inhibit configuration; an empty route alone does not prove that VREF is unavailable.
- After a rejected entry, interpret the message, clear the scratchpad until a read confirms it is empty, verify the documented field/format, and retry the corrected entry once. Repeatedly guessing formats or keys consumes the intercept distance. Read back the accepted flap/VREF selection, not merely typed text.
- If the documented path remains blocked, report it and use an approved weight/configuration performance reference only if available. Do not invent VREF, infer it from takeoff speeds, or mark the FMC-entry item complete without acceptance. If safe landing performance cannot be established, retain a safe flight path and arrange a documented hold or missed approach instead of starting final.
- Set the documented VREF speed correction on the MCP and confirm active thrust mode and actual IAS response. Allow deceleration and scheduled flap extension within the actual maneuver-speed/limit indications. A selected speed alone does not mean the aircraft has slowed. Continue with `737-approach` only with a usable brief and performance data.
