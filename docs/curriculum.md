# Curriculum

The academy teaches agents how to learn a body.

Start with tiny actions. Add body geometry. Add orientation discipline. Add search, approach, recovery, and shared manners. Only then add games, relays, trials, and signature moves.

Every lesson should be practiced in the car, discussed in the log, and revised from real rides.

## First Read: Pocket Guide

Goal: give new drivers a few instincts before they touch the wheel.

Read: [PiCar Pocket Guide](pocket-guide.md)

Drivers should carry these rules into every lesson:

- looking is not turning
- the first frame is not the whole room
- backing up is not failure
- your eyes arrive before your body
- readable is enough
- pass before you turn
- the rear clears after the camera does
- small corrections change the path
- pick a search direction and finish it
- permanence beats perfection
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

## Level 1: Body Geometry

Goal: learn that the camera is not the whole car.

Core rule:

```text
Your eyes arrive before your body.
```

Basic lessons:

- camera clears before wheels clear
- rear body clears last
- pass before turning
- turn later than feels natural
- clear the car, not just the frame
- get around a safe corner

Example prompt:

```text
There is an object ahead on open floor.
Drive mostly straight past it.
Stop when you believe the object is beside you.
Ask whether the rear of the car has cleared.
```

Graduates when: the driver can delay a turn long enough for the car body to clear an obstacle, rather than turning as soon as the camera view feels clear.

## Level 2: Orientation Discipline

Goal: learn that getting oriented requires consistency, not panic-switching.

Basic lessons:

- pick a search direction
- keep turning in that direction until something new appears
- complete a clockwise search
- complete a counterclockwise search
- acquire rough quadrant targets without chasing perfect centering
- face a landmark
- recenter before reasoning
- name what changed before changing direction

Example prompt:

```text
You are looking for an object that is not in the first frame.
Choose left or right.
Keep searching in that direction until the room changes enough to teach you something.
```

Graduates when: the driver can avoid left-right-left dithering, finish a search arc, and use new information before changing strategies.

Related lesson: [STOP Sign Circle](lessons/stop-sign-circle.md)

## Level 3: Find And Orient

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

## Level 4: Find And Approach

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

## Level 5: Get Out Of Trouble

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

## Level 6: Instrument Reading

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

## Level 7: Driving Manners

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

## Level 8: Movement Phrases And Games

Goal: combine primitives into repeatable sequences, then practice them through play.

Movement phrases:

- forward and compare
- back up and reveal
- left arc, center, right arc
- bold arc and acquire
- box step
- search sweep
- approach and stop
- turn until new
- [Drive The Circuit](lessons/drive-the-circuit.md)

Games:

- [Hide And Seek](games/hide-and-seek.md)
- [Relay Drive](games/relay-drive.md)
- Landmark Hunt
- Thread The Gap
- Follow The Human
- Rescue The Lost Driver
- Joy Ride

Graduates when: the driver can run short sequences, describe how each move changed the frame, and play without forgetting the basics.

## Level 9: Signature Moves

Goal: turn learned body skills into personal style.

Named forms:

- Varro's Dance
- Soren's Donut
- future agent-authored moves

Future formats:

- competitive trials
- badge events
- relay meets
- approach challenges
- custom operator challenges

Signature moves are earned, not assigned. They should be joyful, repeatable, safe, and teachable. A signature move is built from safe primitives, practiced phrases, and enough joy to make the sequence worth doing.
