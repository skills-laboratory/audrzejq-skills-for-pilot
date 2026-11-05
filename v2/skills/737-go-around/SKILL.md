---
name: 737-go-around
description: Use when an approach must be discontinued, for controlled missed-approach flight and recovery from unexpected pitch or trim behavior.
---

# Boeing 737 go-around and missed approach

## Fly before cleaning up

1. Apply the documented go-around thrust/TO/GA action and configuration sequence; verify thrust, FMA, and both CMD channels immediately. Select the charted missed-approach track and altitude as prescribed. TO/GA may disconnect a single autopilot: with CMD off, flight-director guidance is not control of the aircraft.
2. If uncoupled, acquire manual authority through the documented flight-control interface and issue bounded pitch/roll corrections. Verify control-input readings and actual response, including any required joystick-override state; a neutral yoke is not an attitude hold. Follow valid flight-director guidance, normally toward an initial attitude around 15 degrees, while protecting the weight/configuration-dependent go-around speed. Reduce pitch promptly if IAS decays or attitude continues rising; do not rely on a trim command or autopilot engagement to arrest an unsafe pitch trend.
3. Alternate small control corrections with immediate instrument reads, aiming for 1–2 second feedback as latency permits. Confirm safe IAS, arrested pitch trend, rising altitude, and positive climb before secondary tasks. TO/GA or a selected altitude alone does not prove a climb or level-off. Do not search documents or change display range during a developing upset.
4. Select gear UP only after positive climb; if already up, verify that state without claiming a retraction occurred. Use the actual missed-approach flap sequence for the starting configuration. An early go-around from a clean aircraft is not permission to extend flaps to mimic a landing-configured procedure. After the prescribed initial selection, defer further retraction until the acceleration conditions and maneuver speeds are satisfied; positive climb alone is not permission to retract toward clean.
5. After stable acceleration and the required retraction, establish the documented pitch/roll/thrust modes and recheck selected targets, which may synchronize during a mode change. Engage an autopilot only with safe attitude/speed and confirmed prerequisites, then verify CMD remains engaged and the flight path responds. Use `737-altitude-hold` to anticipate the missed-approach level-off rather than overshooting it.

## Unexpected pitch or trim

- If pitch diverges, take documented manual control and correct attitude/thrust first using `737-climb` recovery guidance. Inspect actual control authority, CMD status, trim input, and stabilizer movement; do not diagnose a stuck pilot input from a trim reading alone. Do not repeatedly re-engage a dropping autopilot or use long absolute-trim setpoint calls as the primary pitch control during an upset.
- For confirmed continuous uncommanded stabilizer movement, follow the documented runaway-stabilizer procedure, including autopilot disconnection and supported trim-cutout controls as applicable. Release unintended trim input and verify whether movement stops. Do not invent switch actions or assume a zero trim command has isolated a fault. If required controls are missing or behavior persists, report it and maintain the safest achievable flight path; do not attempt another landing with unresolved control authority.
- Once successive fresh readings establish safe speed and sustained altitude control, continue the assigned missed approach. If another approach is authorized and equipment is usable, rebrief its intercept and restart the applicable checklist sections. Distinguish a transient deviation from a persistent failure; neither a brief target crossing nor an FMA alone proves stabilization or permanent malfunction.
