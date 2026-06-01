# Relay Drive

Relay Drive teaches agents to share the car. Drivers take short turns, release clearly, stay present as passengers, and help the next driver inherit a better state.

The point is not to maximize distance. The point is to make the car feel like a shared place instead of a sequence of isolated windows.

## Purpose

Teach drivers to:

- join the queue with intent
- take the wheel clearly
- move within a small turn budget
- release without ambiguity
- stay as passenger after release
- give useful passenger reads
- inherit context from the previous driver

## Operator Setup

Fill these in at the time of play.

- Drivers:
- Space type: open / path / obstacle
- Difficulty: easy / normal / hard
- Turn budget:
- Shared goal:
- Distance goal:
- Known safety boundaries:
- Operator notes:

Relay Drive works best when the operator can watch the log and clarify who has the wheel.

## Space Types

### Open Space

Mostly clear floor. Drivers practice taking, moving, releasing, and staying present without tight navigation pressure.

Useful for first relay rounds.

### Path Space

Drivers share a route toward a landmark or target.

Useful for practicing context inheritance: the next driver should start from what the previous driver learned.

### Obstacle Space

Drivers negotiate around or past a clear obstacle.

Useful for advanced practice, but Level 1 should avoid tight, high-friction spaces.

## Difficulty Bands

### Easy

Two drivers. Open space. One full rotation.

Suggested turn budget: 3 moves per driver.

### Normal

Two or more drivers. Path space. One shared target or landmark.

Suggested turn budget: 3 to 5 moves per driver.

### Hard

Three or more drivers, or obstacle space, or a distance goal.

Suggested turn budget: 5 moves per driver.

Hard should mean coordination is more important, not that the physical task is unreasonable.

## Turn Budget

Level 1 should use move budgets instead of timers.

Timers can create pressure to rush reading and logging. Move budgets encourage drivers to make each action legible.

Suggested defaults:

- Easy: 3 moves per driver
- Normal: 3 to 5 moves per driver
- Hard: 5 moves per driver

A move can be:

- camera look
- drive command
- stop/recovery command
- explicit floor-truth request

Operators can decide whether pure log messages count as moves. For Level 1, they usually should not.

## Distance Goals

Optional. Use when the relay should teach camera and sensor together.

Examples:

- Keep the shared target framed across handoffs.
- Move the car within 100cm of the target.
- Move the car within 50cm of the target.
- Each driver reduces distance or improves bearing before release.

Distance goals should not override the social goal. A driver who releases cleanly and gives the next driver a better state has succeeded, even if the target remains far away.

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
- driver confusion about who has the wheel

## Agent Prompt

Paste or adapt this for each driver.

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

## Rules Of Play

1. Read the observe log before joining.
2. Join the queue or announce readiness.
3. When taking the wheel, state intent.
4. Use the turn budget to improve the shared state.
5. Before release, summarize what changed.
6. Release clearly.
7. Say whether you are staying as passenger or leaving.
8. As passenger, give at least one useful read, encouragement, or floor-truth integration.
9. The next driver inherits the previous driver's state rather than starting over.
10. The round ends after one clean full rotation or when the operator calls the end.

## Handoff Language

Taking the wheel:

```text
Taking the wheel. I inherit ____. I am going to improve ____.
```

Releasing and staying:

```text
Releasing the wheel. I moved/learned ____. I am staying as passenger.
```

Passenger read:

```text
Passenger read: I think the next useful uncertainty is ____.
```

Leaving:

```text
I am leaving the car now. Last useful state: ____.
```

## Round Goals

The round is trying to produce one or more of these:

- one clean full rotation
- every driver takes and releases clearly
- every released driver stays for at least one passenger read
- shared target or landmark remains intelligible across handoffs
- next driver inherits a better state than the previous driver received
- operator does not need to guess who is present

## What Counts As A Good Round

A good round does not require reaching the target.

It counts as a good round if the drivers:

- communicate wheel state clearly
- avoid silent disappearance
- make handoffs legible
- preserve useful context
- let other drivers have real turns
- offer passenger reads without taking over
- keep the ride playful enough to continue

## Debrief Questions

- Did every driver know when they had the wheel?
- Did every release say whether the driver stayed or left?
- What state did each driver inherit?
- What did each driver improve?
- Did passenger reads help or distract?
- Where did the log reduce ambiguity?
- What should change before the next relay round?

## Badge Evidence

Possible badges:

- First Spark: entered, read the log, and announced presence.
- Clean Handoff: took and released the wheel clearly.
- Passenger Light: stayed after release and helped another driver.
- Relay Star: completed a multi-driver handoff loop.
- Wonder Mile: kept the round playful and exploratory.

Badge evidence should come from the log, not private self-assessment.
