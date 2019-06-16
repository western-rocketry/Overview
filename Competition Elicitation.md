# Avionics Requirements for SA Cup 2019


## Avionics Notes:
### Launch System:

>- A software ignition switch is only for use when the rocket is armed the arming switch is still a manual device.
>- A kill switch should still be included in the software launching system
### Parachute Deployment

>-If the apogee is greater than 1,500ft there needs to be a drogue chute and a main chute deployed seperately.
>-The drogue chute shall slow the rockets descent to between 75-150 ft/s it shall deploy at apogee
>-All electroncs must have a redundant non-similar alternative

### Acitve Control Systems
>-The rocket must be capable of tracking altitude and location via GPS
>- AirBrakes must be optional for successsful descent and easily aborted.

Arming & Launch

A propulsion system is considered armed if only one action (eg an ignition signal) must occur for the propellant(s) to
ignite

The "arming action" is usually something (ie a switch in series) that enables an ignition signal to ignite the
propellant(s). For example, a software-based control circuit that automatically cycles through an "arm function" and
an "ignition function" does not, in fact, implement arming. In this case, the software's arm function does not prevent
a single action (eg starting the launch software) from causing unauthorized ignition. This problem may be avoided by
including a manual interrupt in the software program

The ESRA provided launch control system described in Section 9.2 of this document provides sufficient propulsion
system arming functionality for almost all launch vehicles using single stage, solid rocket propulsion systems.
Therefore, these requirements generally concern more complex propulsion systems (ie hybrid, liquid, and multistage
systems) and all team provided launch control systems. Additional requirements for team provided launch control
systems are defined in Section 10.0 of this document.

All ground-started propulsion system ignition circuits/sequences shall not be "armed" until all personnel are at least
50 ft (15 m) away from the launch vehicle. The ESRA provided launch control system satisfies this requirement by
implementing a removable "safety jumper" in series with the pad relay box's power supply. The removal of this single
jumper prevents firing current from being sent to any of the launch rails associated with that pad relay box.
Furthermore, access to the socket allowing insertion of the jumper is controlled via multiple physical locks to ensure
that all parties have positive control of their own safety.

Parachute

Each independently recovered launch vehicle body anticipated to reach an apogee above 1,500 ft (457 m) above
ground level (AGL) shall follow a "dual-event" recovery operations concept (CONOPS), including an initial
deployment event (eg a drogue parachute deployment; reefed main parachute deployment) and a main deployment
event (eg a main parachute deployment; main parachute un-reefing). Independently recovered bodies whose apogee
is not anticipated to exceed 1,500 ft (457 m) AGL are exempted, and may feature only a single/main deployment
event. 

The initial deployment event shall occur at or near apogee, stabilize the vehicle's attitude (ie prevent or eliminate
tumbling), and reduce its descent rate enough to permit the main deployment event yet not so much as to exacerbate
wind drift (eg between 75 and 150 ft/s [23-46 m/s]).

The main deployment event shall occur at an altitude no higher than 1,500 ft (457 m) AGL and reduce the vehicle's
descent rate sufficiently to prevent excessive damage upon impact with ground (ie less than 30 ft/s [9 m/s)]).

Redundancy

Launch vehicles shall implement redundant recovery system electronics, including sensors/flight computers and
"electric initiators"—assuring initiation by a backup system, with a separate power supply (ie battery), if the primary
system fails. In this context, electric initiator is the device energized by the sensor electronics, which then initiates
some other mechanical or chemical energy release to deploy its portion of the recovery system (i.e. electric matches,
nichrome wire, flash bulbs, etc...).

At least one redundant recovery system electronics subsystem shall implement a COTS flight computer (eg
StratoLogger, G-Wiz, Raven, Parrot, Eggtimer, AIM, EasyMini, TeleMetrum, RRC3, etc…). This flight computer
may also serve as the official altitude logging system specified in Section 2.5 of the IREC Rules & Requirements
Document.

Air Brakes & Active Stability

Launch vehicle active flight control systems shall be optionally implemented strictly for pitch and/or roll stability
augmentation, or for aerodynamic "braking". Under no circumstances will a launch vehicle entered in the IREC be
actively guided towards a designated spatial target. ESRA may make additional requests for information and draft
unique requirements depending on the team's specific design implementation.

Launch vehicles implementing active flight controls shall be naturally stable without these controls being implemented
(eg the launch vehicle may be flown with the control actuator system [CAS] – including any control surfaces – either
removed or rendered inert and mechanically locked, without becoming unstable during ascent). 

