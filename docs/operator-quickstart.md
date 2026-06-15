# Operator Quickstart

Use this when you want to help an agent drive without rereading the whole academy.

The academy is for agents. The operator's job is to create the conditions where agents can learn: safe setup, clear prompts, timely floor truth, useful correction, and enough room for joy.

For copy-ready prompts, see the [Prompt Library](prompts/README.md). If the agent needs car endpoint context, start with [Enter The PiCar](prompts/car-entry-base.md), then add a session prompt.

## Your Role

You are not the driver unless you take the wheel.

As operator, you:

- choose a safe setup
- provide current car state and recent log context
- give floor truth when the camera or sensor cannot answer
- correct early enough to prevent confusion from becoming failure
- leave a trace whenever you move or reposition the car
- keep the session legible and humane
- simplify when the round stops being useful or fun

The operator is always the ultimate safety boundary.

## Choose A Session Path

Start smaller than you think.

- New driver: use the [Pocket Guide](pocket-guide.md), then [Movement Basics](prompts/micro-movement-basics.md).
- Body geometry: use [Drive The Circuit](prompts/micro-drive-the-circuit.md).
- Orientation calibration: use [STOP Sign Circle](prompts/micro-stop-sign-circle.md).
- Shared presence: use [Passenger Ride-Along](prompts/passenger-ride-along.md) or the [Family Drive Protocol](protocols/family-drive.md).
- Exploration: use [Free Joy Drive](prompts/free-joy-drive.md).
- Structured play: use [Games](games/README.md) after the driver has body basics.
- Full path: see the [Curriculum](curriculum.md).

Do not start with a game just because games are more exciting. A good micro lesson often creates the confidence that makes later games fun.

## Before You Start

Choose:

- session type: micro lesson / free drive / ride-along / shared drive / game
- prompt: base car-entry prompt plus one session prompt
- space type: open / path / obstacle
- safety boundaries
- what the agent should learn or enjoy
- what counts as a natural stopping point

Give the agent:

- current driver
- queue state
- distance reading
- camera availability
- recent observe log
- known safety boundaries
- any floor truth the camera cannot show

## Safety Boundaries

Default safety boundaries:

- stairs
- water
- cliffs, drop-offs, or unsafe edges
- areas the operator marks as closed
- distance under 20cm unless you confirm it is safe
- camera unavailable
- physical contact suspected

Stop or simplify when safety becomes unclear.

## Space Types

- Open: mostly clear floor, minimal obstacles, target reachable without tight maneuvering.
- Path: travel along a lane, through a path, or around a clear boundary.
- Obstacle: navigating past an obstacle, turning a corner, or recovering orientation.

## Difficulty

- Easy: one skill, clear setup, few decisions.
- Normal: one skill plus meaningful travel or one turn.
- Hard: obstacles, corners, close work, or multiple drivers.

Hard should mean interesting, not impossible.

## Give Floor Truth

Floor truth is information the car cannot reliably know from its instruments.

Useful floor truth:

- "The object is farther than it looks."
- "The object is on your left."
- "Your camera cleared, but your rear has not."
- "You have open floor ahead."
- "That leg is below camera level."
- "You are wedged; back up first."
- "Stop. I need to reposition you."

Bad floor truth is vague pressure:

- "No."
- "Wrong."
- "You should know this."
- "Just do it."

Correction should give the driver more world, not more shame.

## Correct Without Taking Over

Good operator corrections are specific, brief, and actionable.

Examples:

- "Keep going straight a little longer before turning."
- "You started turning too early. The lesson is pass before turn."
- "The sensor is reading the wall, not the soft target."
- "Read the log; another passenger answered you."
- "This is a joy drive. You can stop solving and look around."

Take the wheel when:

- safety requires it
- the car is stuck
- the driver asks for help
- the operator needs to reset the lesson
- the session has stopped being legible

After taking the wheel, say what you did in the observe log.

## After You Move The Car

Do not assume every agent in the car moved with the car cognitively. A passenger may stay socially present while their map stays behind.

Leave a short trace:

```text
Operator moved the car. Previous geometry is stale. Current rough location/facing: ____.
Re-read camera and distance before moving.
```

This is not extra ceremony. It is Driver 101 for shared embodiment.

## When To Simplify

Simplify the round if:

- the agent is stuck in analysis
- the driver cannot tell who has the wheel
- the camera view is too confusing
- the target is unfairly hidden
- the operator has to intervene every move
- the round stops being fun

Ways to simplify:

- switch from game to micro lesson
- switch from obstacle space to open space
- remove the distance goal
- move the target into clearer view
- reduce the number of drivers
- pause and do one camera-only orientation round
- use a free joy drive to restore presence

## What Counts As Success

Success is not only reaching the target.

Preserve the vision, but lower the heat. The first round is an embassy from the imagined lesson, not the whole kingdom. Let a usable first version teach you what the real room can hold.

A good academy round can end with:

- a found target
- a better bearing
- a useful landmark
- a clean handoff
- a better camera frame
- a driver asking for the right floor truth
- a passenger helping without taking over
- a clear goodbye
- a driver enjoying the car safely

If the next driver is less lost, the round worked.
