---
name: 737-checklist
description: Use before movement and at each procedure transition to execute and record verified Boeing 737 checklist items.
---

# Boeing 737 checklist execution

1. Use `list_checklist_categories` and `read_checklist` to obtain the live category, sections, item identifiers, conditions, and expected responses. Read each section when its procedure becomes applicable. Use the tools' current schema to establish the active section if required; do not assume section transitions are automatic.
2. Use the default authenticated context unless the tool requires an explicitly supplied identifier. Never invent user or run identifiers. On an access failure, retry with the supported default context; if still blocked, report the issue and continue the physical procedure safely without claiming recorded completion.
3. For each item: establish its stated condition, perform or verify the action, read the relevant aircraft indications, then call `mark_checklist` with the live identifiers and required response. Record each evidenced item independently; do not wait for the entire section or a successful landing. A go-around or unfinished segment does not erase earlier verified preparation, but does not justify marking the failed or unverified items. Reading a procedure or changing a switch does not record completion.
4. Verify that the mark is accepted and that checklist progress changes. Acceptance records your assertion; it does not supply missing aircraft evidence. Before leaving a section, read it back and resolve unmarked applicable items. Do not mark future, unverified, or failed actions complete; a historical trigger must have been observed, not inferred from the present state.
5. Prepare the upcoming airborne items while stopped or in verified stable automated flight. During low final, rotation, or recovery, aircraft control takes priority; retain the verified evidence and record it at the next safe opportunity without leaving a sustained control input unattended. Before final, or after a stabilized go-around, read progress and reconcile applicable verified items rather than deferring all marking to task completion.

## Takeoff conditions to preserve

- Before runway entry, verify actual runway identity and runway-entry authority. In a runway-loaded scenario, verify the initial runway and the scenario's stated authority rather than inventing a prior clearance.
- At entry, verify the required strobe/other lights and both transponder code and mode. After takeoff authority, verify the required fixed landing lights and approximately 40% N1 on both engines.
- After engine stabilization, verify TO/GA outcome; at the applicable VR, verify rotation toward 15°; at positive climb, verify gear retraction.
- Above the procedure's stated 400 ft datum, verify the permitted roll mode and scheduled flap retraction. Height alone does not establish safe flap-retraction speed.
- Only after actual flap/slat retraction, complete the prescribed VNAV selection, autopilot decision, engine start-switch positions, autobrake OFF, and gear-lever OFF checks. Verify actual modes and configuration, not just switch commands.
- For gear-lever OFF, retracted gear and a handle-not-down indication do not distinguish UP from OFF. Require evidence that distinguishes the OFF detent. If the selection remains unverified and no such indication is available, leave that item unmarked and report the limitation while continuing safe flight; reporting it does not justify marking it complete.
