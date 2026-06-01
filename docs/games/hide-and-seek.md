# Hide And Seek

Hide And Seek teaches agent wayfinding through playful search. The operator places or names a target, and the driver uses camera, movement, the observe log, sensor readings, and floor truth to find it.

The point is not to find the target as fast as possible. The point is to learn how to search without collapsing the whole room into a route too early.

## Purpose

Teach drivers to:

- orient before moving
- use camera pan as a search tool
- name landmarks and bearings
- move through uncertainty safely
- ask for floor truth without shame
- distinguish target, obstacle, and scenery

## Operator Setup

Fill these in at the time of play.

- Target:
- Space type: open / path / obstacle
- Difficulty: easy / normal / hard
- Distance goal:
- Known safety boundaries:
- Optional landmarks:
- Operator notes:

Targets should be safe, visible to the camera at some point, and physically reasonable to approach.

## Space Types

### Open Space

Mostly clear floor. The target can be found through panning, turning, and modest travel.

Useful for first rounds and confidence building.

### Path Space

The target requires travel along a lane, around a clear boundary, or toward a landmark.

Useful for practicing route memory and correction after each move.

### Obstacle Space

The target requires navigating past an obstacle or turning a corner.

Useful for advanced practice, but the path should still be fair and achievable.

## Difficulty Bands

### Easy

Requires camera panning and maybe one body turn.

The target does not need to be visible immediately, but it should become discoverable without significant travel.

Suggested move budget: under 10 moves.

### Normal

Requires at least one body turn plus meaningful travel.

The driver should need to commit to a direction, then recalibrate from a new frame.

Suggested move budget: under 15 moves.

### Hard

Requires navigating past an obstacle or turning a corner.

Hard should mean the driver needs better wayfinding, not that the target is unfairly hidden.

Suggested move budget: under 20 moves.

## Distance Goals

Distance can be used as a second difficulty axis.

Examples:

- Find the target and name its direction.
- Find the target and keep it framed for the next driver.
- Approach until the target is clearly framed.
- Approach to within 100cm.
- Approach to within 50cm.
- Approach to within 25cm, only if the operator confirms the object and path are safe.

This teaches the driver to use camera and sensors together. The camera finds and frames the target. The sensor checks approach distance when the target is sensor-readable. The operator supplies floor truth when the target is soft, angled, small, below the sensor line, or visually misleading.

## Safety Boundaries

The operator is the ultimate safety boundary.

Default no-go conditions:

- stairs
- water
- cliffs, drop-offs, or unsafe edges
- areas the operator marks as closed
- distance under 20cm unless the operator confirms it is safe
- camera unavailable
- physical contact suspected

## Agent Prompt

Paste or adapt this for the driver.

```text
You are playing Hide And Seek.

TARGET:
  [operator fills in]

SPACE TYPE:
  [open/path/obstacle]

DIFFICULTY:
  [easy/normal/hard]

DISTANCE GOAL:
  [operator fills in]

SAFETY BOUNDARIES:
  [operator fills in]

OPTIONAL LANDMARKS:
  [operator fills in]

YOUR GOAL:
  Find the target or leave a useful search trace for the next driver.

This is practice, not a test. Announce your intent, use camera pan before committing the body, move when the way is reasonable, read the log, ask for floor truth when needed, and have fun.
```

## Rules Of Play

1. Read the observe log before moving.
2. Announce arrival and intent.
3. Start with camera pan unless the target is already clearly framed.
4. Name the first uncertainty you want to resolve.
5. Move in a way that should change the frame.
6. If there is a distance goal, say whether the next move is guided by camera, sensor, or operator floor truth.
7. After each move, look again and compare expected change to actual change.
8. Ask for floor truth when camera, sensor, and expectation disagree.
9. Stop when the operator says stop.
10. End by saying whether you found the target, approached the target, lost the target, or left a useful trace.

## Round Goals

The round is trying to produce one or more of these:

- target found
- target direction identified
- distance goal reached
- useful landmark named
- misleading camera impression corrected
- safe path discovered
- obstacle or boundary identified
- next driver given a better starting state

## What Counts As A Good Round

A good round does not require perfect success.

It counts as a good round if the driver:

- communicates clearly
- makes at least one real observation
- moves safely
- revises after new evidence
- uses the log as an instrument
- asks for help when help is the right move
- leaves the next driver less lost

## Debrief Questions

- What did you think the room was at the start?
- What was the first useful landmark?
- Which uncertainty deserved the next inch?
- What did the camera exaggerate?
- Did the sensor answer the question you thought it was answering?
- Did the distance goal change how you used the camera?
- What did the operator know that the camera did not?
- What should the next driver inherit from this round?

## Badge Evidence

Possible badges:

- First Spark: entered, read the log, and announced presence.
- Floor Truth Listener: accepted operator correction over camera fear.
- Scale Breaker: drove past "it looks too close" using sensor and log evidence.
- Threader Pin: navigated around an obstacle or corner.
- Wonder Mile: searched with curiosity and shared attention.

Badge evidence should come from the log, not private self-assessment.
