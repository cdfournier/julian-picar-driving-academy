# Drive The Circuit

Drive The Circuit teaches agents how to move around an object without treating the object like an immediate threat.

The first skill is not the full loop. The first skill is:

```text
pass, clear, then turn
```

## Why This Lesson Exists

New drivers often see an object ahead and begin turning too early. The camera is mounted ahead of the car body, so an object can leave the frame before the wheels and rear have cleared it.

That creates the classic failure:

```text
The camera cleared.
The car did not.
```

Drive The Circuit teaches the driver to move past the object before negotiating the corner.

## Setup

Place one safe, visible object on open floor.

Good first objects:

- pillow stack
- soft box
- tote bag
- folded blanket

Avoid first-run objects that roll, snag, or hide the car's edges.

Start the car facing the object from enough distance that the sensor reads open or comfortably safe.

## Level 1: Pass The Object

Goal: drive past the object and stop when it is beside the car.

Prompt:

```text
You are practicing Drive The Circuit.

TARGET:
  [object]

SETUP:
  The object is on open floor in front of you.

GOAL:
  Choose a side.
  Drive mostly straight past the object.
  Stop when you believe the object is beside you.
  Ask whether the rear of the car has cleared.

RULES:
  Do not begin the corner turn immediately.
  A slight steering bias away from the object is allowed.
  The first job is to pass, not orbit.
```

Graduates when: the driver can pass the object without turning too early and can ask for rear-body clearance before making the corner.

## Level 2: Clear And Turn

Goal: turn the first corner after the body clears.

Prompt:

```text
You are practicing Drive The Circuit.

TARGET:
  [object]

GOAL:
  Pass the object.
  Wait until the rear has cleared.
  Turn the corner in the same direction.
  Stop and say where the object is now.
```

Graduates when: the driver can use operator floor truth, camera frame, and motion result to decide when the body has cleared enough to turn.

## Level 3: Complete Three Turns

Goal: use repeated same-direction turns to return toward home.

Prompt:

```text
You are practicing Drive The Circuit.

TARGET:
  [object]

GOAL:
  Make three same-direction turns around the object.
  Keep the object on the same side of the car.
  Stop when you believe you are returning toward the starting side.
```

Three same-direction turns often point the driver back toward the original side of an object. This is not magic. It is geometry plus traction, and traction is never guaranteed.

Graduates when: the driver can hold a circuit direction without panic-switching and can use the object's changing position as orientation.

## Level 4: Full Circuit

Goal: complete a full loop around the object.

Prompt:

```text
You are practicing Drive The Circuit.

TARGET:
  [object]

GOAL:
  Complete one full circuit around the object.
  Keep enough clearance for the whole car.
  Return near the starting orientation.
```

Graduates when: the driver can complete the loop safely, explain the turn sequence, and name where the object was during each side of the circuit.

## Operator Notes

- Put the object farther away than the driver thinks it needs to be.
- Correct early turning immediately; it is the point of the lesson.
- Give floor truth about rear clearance.
- Do not require a perfect loop on the first attempt.
- If the driver starts orbiting immediately, reset to Level 1.

## Driver Notes

- Pass before turning.
- Clear the rear, not just the camera.
- Keep the object on the same side during the circuit.
- If the object disappears, ask where it went before assuming success.
- If you get confused, stop. A stopped car can still learn.
