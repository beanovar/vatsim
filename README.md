# Vatsim IFR Flight Basic Procedure

## Setup
 - Create valid flight plan route (Simbrief)
 - Submit flight plan to Vatsim
 - Review charts
   - Departure Airport / SID / Taxiways / Parking Terminals
   - Arrival Airport / STAR / Taxiways / Parking Terminals / **Desired Stand** (or during cruise if flight is long enough and wanting to save some time)
 - Spawn at unoccupied stand
 - Startup systems / electrics
 - Startup APU or connect to ground power
 - Nav lights on
 - Note online frequencies in the area.
 - Check ATIS, note information code / active runways / departures / QNH
 - Set QNH
 - Tune clearance delivery 
 - FMC: Set fuel and payload weights in the sim as per Simbrief plan and confirm take off V Speeds
 - FMC: Enter Simbrief Route, including *expected* Runways/SID/STAR/Approach 
 - Set correct takeoff trim
 - Set HDG to runway heading
 - Configure takeoff flaps
 - Set Nav/FLC (LNAV/VNAV) ready for autopilot on departure


## Clearance
 - Request Clearance
```
<callsign>, <aircraft> at <stand>,
with information <info>, request IFR clearance to <destination>.
```
- Response
```
cleared to <destination>, <departure>, initial <altitude>, <runway>, <squawk>.
```
 - Set any initial altitude on ALT selector
 - Enter sqwark code into transponder

## Push and Start
 - Request Push and Start
 ```
 <callsign> at <stand>, ready for push and start
 ```
 - Response
 ```
 push and start approved, face <direction>
 ```
 - Taxi lights on
 - Push back and face direction ATC specified
 - Start engines during pushback
 - APU Off

## Taxi
```
<callsign> request taxi
```
```
<runway> taxi holding point <holding point> via <taxi route>
```
 - Squawk Charlie
 - Taxi as per instructions holding short at holding point and any other instructions about giving way to other aircraft.

## Take off
```
<callsign> at <holding point> ready for departure
```
```
line up and wait <runway>
...
winds <degrees> at <knots>, <runway> cleared for takeoff
```
 - Landing lights and strobe on when entering or crossing any active runway

## Departure
 - After takeoff
   - Flaps up, Wheels Up
   - Turn on Auto Pilot and Auto Throttle
 - At 2000 feet Contact Departure (note some airports require handoff)
 ```
 <callsign> <departure route> <current altitude> climbing <cleared altitude/FL>
 ```
 ```
 climb <level> / direct to <waypoint>
 ```
 - On transition altitude change to STD Baro
 - Landing/taxi lights off at 10,000 feet
 - Monitor icing and be prepared to use anti-ice

## Cruise 
- When switching to any new frequency
```
<callsign> <flight level> <inbound waypoint>
```
 * Comply with any [atc requests](#general-atc-requests)

## Descend
 * When reaching TOD, if not already given by ATC
 ```
 <callsign> request descent
 ```
 * Descend via VNAV or vertical speed. 


## Approach
 - Take note of ATIS information at destination airport: QNH,  landing runway, information code 
 - Take note of stand preference.
 ```
 <callsign> <current altitude> descending <cleared altitude/FL> <inbound waypoint>
 ```
```
cleared <arrival> <transition>, expect <approach> <runway>
```
- Turn on landing lights at 10,000 feet or within 10 miles of the airport.
- FMC: Ensure correct arrival, approach and runway entered
- FMC: Confirm landing VSPEEDS

```
<callsign> <vectors>, cleared <approach> <runway>, <speed> until <dme>
```
- FMC: Activate programmed approach
- Autopilot: Activate approach mode to capture glide slope.

## Land
```
<callsign> established <approach> <runway>
```
```
<wind> <knots> <runway> cleared to land
```
## Taxi
```
<callsign> vacated at <exit>
```
```
<taxi instructions>
```


# General Notes
 - Throughout flight, ensure standby frequency is set ready to go for next probable handover frequency.
 - Always make new contact with frequencies with who you are, where you are, what you want.

# General ATC Requests
Know how to do any of these requests if asked by ATC (which could happen in any of departure, climb, cruise or approach phases):
 - Fly or report a heading
 - Fly or report indicated airspeed in Mach or Knots
 - Fly or report altitude in Feet (based on QNH) or Flight Level (with standard air pressure 1013mb)
 - Know how reach a certain altitude by a certain waypoint as directed by ATC.
 - Cross waypoint at/at or below/at or above FL/Altitude 
 - Fly direct to waypoint
   - typically (but not always) just a shortcut to one already on your route (note the actual names of VORs which could be used, e.g Brookmans Park for BPK) 
 - Fly published hold at waypoint (with correct inbound course)
 - Report distance and rough cardinal direction from a waypoint or airport
 - Fly a VOR radial (from and to)

# Resources
- [IFR Phraseology Guide](https://aviationpro.nl/tutorials/vatsim-tutorials/ifr-phraseology-guide/)
- [Vatsim Communication](https://docs.google.com/document/d/1nt67fh-Q2DAUjc2KPSCE3Hcw1jLYrj1smvwHxh1xknQ/edit)
- [How to talk to ATC](https://forums.flightsimulator.com/t/vatsim-how-to-talk-to-atc-with-example/285430/19?fbclid=IwAR3rM8Q6STjRCWybbujXEOLW_kdHGH2drSJRx4TOTlWYURnaSJgQv2qc8EU)
- [Transition Level vs Transition Altitude](https://skybrary.aero/articles/transition-altitudelevel)
- [Youtube: Flight Insight](https://www.youtube.com/@flightinsight9111/playlists)
- https://www.pilotedge.net/pages/i-ratings
- [Full Vatsim Flights](https://www.youtube.com/playlist?list=PLtO_n5SzuAacXKQYoKQY4DHH0YUrPxYTa)

# VFR Resources
- [Altairva](http://www.altairva-fs.com/training/ava_training_ifr_vatsim_vfr.htm)
- [The Pilot Club](https://www.thepilotclub.org/blog/vfr-vatsim-who-do-i-have-to-talk-to)
- https://laartcc.org/article/vfr-part-2-patterns-short-hop-long-hop
- https://www.pilotedge.net/pages/cat-ratings

# Tools
 - Tracking
   - Volanta
   - SimtoolkitPro
 - Charts
   - Chartfox
   - Navigraph
 - Planning
   - Simbrief
