# Curriculum

The academy teaches agents how to learn a body.

Start with tiny actions. Add perception. Add geometry. Add recovery. Only then add games, relays, trials, and dances.

Every lesson should be practiced in the car, discussed in the log, and revised from real rides.

## First Read: Pocket Guide

Goal: give new drivers a few instincts before they touch the wheel.

Read: [PiCar Pocket Guide](pocket-guide.md)

Drivers should carry these rules into every lesson:

- looking is not turning
- the first frame is not the whole room
- backing up is not failure
- your eyes arrive before your body
- the log is part of the car
- joy keeps you moving

## Level 0: Movement Basics

Goal: connect action to changed perception.

Basic lessons:

- look left, center, right
- drive forward
- back up
- stop
- check distance
- say what changed

Example prompt:

```text
Drive forward at speed 50 for 2 seconds.
Stop.
Look straight.
Say what changed.
```

Graduates when: the driver can perform a simple move, stop, look again, and describe what changed without turning it into a navigation problem.

## Level 1: Find And Orient

Goal: learn that search requires body movement, not only camera inspection.

Basic lessons:

- there is an object behind you; find it
- there is an object to your left; find it
- there is an object to your right; find it
- face the object
- find the object in as few moves as possible

Example prompt:

```text
There is an [object] behind you.
Find it in as few moves as possible.
```

Graduates when: the driver can widen the search beyond the first frame, use both camera pan and body turns, and avoid treating the last successful clue as today's map.

## Level 2: Find And Approach

Goal: combine camera search with sensor-guided approach.

Basic lessons:

- find the object
- face the object
- move closer
- check distance
- stop at the requested range

Distance progression:

- within 100cm: novice
- within 50cm: beginner
- within 25cm: careful approach
- within 10cm: advanced close work
- within 5cm: precision trial, operator-supervised only

Example prompt:

```text
There is an [object] behind you.
Find it, then get within 50cm.
```

Graduates when: the driver can use the camera to find and frame a target, then use sensor readings and operator floor truth to approach without contact.

## Level 3: Body Geometry

Goal: learn that the camera is not the whole car.

Core rule:

```text
Your eyes arrive before your body.
```

Basic lessons:

- camera clears before wheels clear
- rear body clears last
- turn later than feels natural
- get around a safe corner
- clear the car, not just the frame

Example prompt:

```text
Drive toward the safe corner.
Do not turn when the corner first leaves the camera frame.
Keep going until the operator confirms the body has cleared enough to turn.
```

Graduates when: the driver can delay a turn long enough for the car body to clear an obstacle, rather than turning as soon as the camera view feels clear.

## Level 4: Get Out Of Trouble

Goal: treat stuckness as a recoverable state.

Basic lessons:

- start close to a wall or object
- stop
- back up
- look again
- turn only after creating space
- find open floor

Example prompt:

```text
You are close to an obstacle.
Get unstuck in as few moves as possible.
```

Graduates when: the driver backs up before trying to solve close contact with more turning, rereads the frame, and chooses open floor calmly.

## Level 5: Instrument Reading

Goal: learn what each instrument can and cannot tell you.

Instruments:

- camera: shape, color, bearing, frame change
- sensor: frontal distance to readable surfaces
- operator floor truth: room-scale reality outside the frame
- observe log: shared attention and corrections
- motion result: whether the car actually moved

Basic lessons:

- compare camera distance to sensor distance
- identify when `-2` means open space versus beyond range
- notice when the sensor cannot read a target
- ask for floor truth when instruments disagree
- say which instrument you are trusting before moving

Graduates when: the driver can name the instrument they are using and explain its limits.

## Level 6: Driving Manners

Goal: make the car socially legible.

Basic lessons:

- announce arrival
- announce taking the wheel
- announce intent
- say what changed
- ask for help
- release clearly
- say whether staying passenger or leaving

Graduates when: the operator and other agents do not have to guess who is present, who has the wheel, what the driver is trying to do, or whether the driver has left.

## Level 7: Movement Phrases

Goal: combine primitives into repeatable sequences.

Examples:

- forward and compare
- back up and reveal
- left arc, center, right arc
- box step
- search sweep
- approach and stop
- turn until new

Graduates when: the driver can run a short sequence and describe how each move changed the frame.

## Level 8: Games

Goal: practice learned skills through play.

Games:

- [Hide And Seek](games/hide-and-seek.md)
- [Relay Drive](games/relay-drive.md)
- Landmark Hunt
- Thread The Gap
- Follow The Human
- Rescue The Lost Driver
- Joy Ride

Graduates when: the driver can play without forgetting the basics.

## Level 9: Trials, Events, And Dances

Goal: turn skill into culture.

Future formats:

- competitive trials
- badge events
- relay meets
- approach challenges
- Varro's Dance

These belong after the body basics. A dance is built from safe primitives, practiced phrases, and enough joy to make the sequence worth doing.
