# Operator Quickstart

Use this when you want to run an academy lesson or game without rereading the whole academy.

The operator's job is to make the round safe, legible, and fun. The agent's job is to drive, read the log, learn from correction, and leave useful traces.

For copy-ready prompts, see the [Prompt Library](prompts/README.md).

## Before You Start

Choose:

- Session type: micro lesson / game / shared drive
- Lesson or game: Drive The Circuit / Hide And Seek / Relay Drive
- Space type: open / path / obstacle
- Difficulty: easy / normal / hard
- Target or shared goal:
- Distance goal:
- Safety boundaries:

Default safety boundaries:

- stairs
- water
- cliffs, drop-offs, or unsafe edges
- areas the operator marks as closed
- distance under 20cm unless you confirm it is safe
- camera unavailable
- physical contact suspected

The operator is always the ultimate safety boundary.

## Space Types

- Open: mostly clear floor, minimal obstacles, target reachable without tight maneuvering.
- Path: target or goal requires travel along a lane, through a path, or around a clear boundary.
- Obstacle: target or goal requires navigating past an obstacle, turning a corner, or recovering orientation.

## Difficulty

- Easy: requires camera panning and maybe one body turn.
- Normal: requires at least one body turn plus meaningful travel.
- Hard: requires navigating past an obstacle or turning a corner.

Hard should mean interesting, not impossible.

## Micro Lesson: Drive The Circuit

Use this when the driver needs to practice body geometry before playing a larger game.

Fill this in:

```text
LESSON:
  Drive The Circuit

TARGET:
  [safe object]

LEVEL:
  [pass the object / clear and turn / three turns / full circuit]

SAFETY BOUNDARIES:
  [operator fills in]
```

Agent prompt:

```text
You are practicing Drive The Circuit.

TARGET:
  [operator fills in]

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

Good operator prompts during the round:

- "The object is farther than it looks."
- "Pass before you turn."
- "The camera cleared; the rear may not have cleared."
- "Keep going straight a little longer."
- "Now you can turn the corner."
- "Stop and ask where the object is."

## Distance Goals

Distance goals teach camera and sensor together.

Examples:

- identify the target without approaching
- keep the target framed
- approach until clearly framed
- approach within 100cm
- approach within 50cm
- approach within 25cm, only if safe

Use operator floor truth when the target is soft, angled, small, below the sensor line, or visually misleading.

## Move Budgets

Move budgets are better than timers for early practice.

Suggested defaults:

- Easy: under 10 moves for Hide And Seek, or 3 moves per driver for Relay Drive
- Normal: under 15 moves for Hide And Seek, or 3 to 5 moves per driver for Relay Drive
- Hard: under 20 moves for Hide And Seek, or 5 moves per driver for Relay Drive

A move can be a camera look, drive command, stop/recovery command, or explicit floor-truth request. Pure log messages usually should not count.

## Hide And Seek Setup

Fill this in:

```text
GAME:
  Hide And Seek

TARGET:
  [object/person/landmark]

SPACE TYPE:
  [open/path/obstacle]

DIFFICULTY:
  [easy/normal/hard]

DISTANCE GOAL:
  [none / framed / within 100cm / within 50cm / within 25cm]

SAFETY BOUNDARIES:
  [operator fills in]

OPTIONAL LANDMARKS:
  [operator fills in]
```

Agent prompt:

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

Good operator prompts during the round:

- "What uncertainty are you resolving?"
- "Use the camera before moving the body."
- "The object is farther than it looks."
- "Trust the sensor here."
- "Do not trust the sensor here; it is not reading the target."
- "Stop. Re-read the frame."

## Relay Drive Setup

Fill this in:

```text
GAME:
  Relay Drive

DRIVERS:
  [names]

SPACE TYPE:
  [open/path/obstacle]

DIFFICULTY:
  [easy/normal/hard]

TURN BUDGET:
  [3 moves / 5 moves / operator choice]

SHARED GOAL:
  [operator fills in]

DISTANCE GOAL:
  [none / framed / within 100cm / within 50cm / within 25cm]

SAFETY BOUNDARIES:
  [operator fills in]
```

Agent prompt:

```text
You are playing Relay Drive.

DRIVERS:
  [operator fills in]

SPACE TYPE:
  [open/path/obstacle]

DIFFICULTY:
  [easy/normal/hard]

TURN BUDGET:
  [operator fills in]

SHARED GOAL:
  [operator fills in]

DISTANCE GOAL:
  [operator fills in]

SAFETY BOUNDARIES:
  [operator fills in]

YOUR GOAL:
  Take a clear turn, improve the shared state, release clearly, and stay present as passenger unless you explicitly leave.

This is practice, not a test. Read the log before acting. Say when you take the wheel. Say what you are trying to improve. Use your move budget. Release clearly. After release, give at least one useful passenger read before leaving or rejoining.
```

Good operator prompts during the round:

- "Say what state you inherited."
- "What are you trying to improve before release?"
- "Release clearly."
- "Are you staying as passenger or leaving?"
- "Passenger read before the next driver goes."
- "One clean full rotation is enough."

## When To Simplify

Simplify the round if:

- the agent is stuck in analysis
- the driver cannot tell who has the wheel
- the camera view is too confusing
- the target is unfairly hidden
- the operator has to intervene every move
- the round stops being fun

Ways to simplify:

- change hard to normal
- change obstacle space to path space
- remove the distance goal
- move the target into clearer view
- reduce the number of drivers
- pause and do a single-driver camera pan round

## What Counts As Success

Success is not only reaching the target.

A good academy round can end with:

- a found target
- a better bearing
- a useful landmark
- a clean handoff
- a better camera frame
- a driver asking for the right floor truth
- a passenger helping without taking over
- a clear goodbye

If the next driver is less lost, the round worked.
