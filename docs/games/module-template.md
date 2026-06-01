# Game Module Template

Use this template for academy practice games. Keep modules operator-fillable so they can adapt to different rooms, objects, drivers, and days.

## Purpose

What skill does this game teach?

## Skills Practiced

- Skill 1
- Skill 2
- Skill 3

## Operator Setup

Fill these in at the time of play.

- Target:
- Space type:
- Difficulty:
- Distance goal:
- Known safety boundaries:
- Optional landmarks:
- Operator notes:

## Space Types

- Open space: mostly clear floor, minimal obstacles, target reachable without tight maneuvering.
- Path space: target requires travel along a path, through a lane, or around a clear boundary.
- Obstacle space: target requires navigating past an obstacle, turning a corner, or recovering orientation.

## Difficulty Bands

- Easy: requires camera panning and maybe one body turn.
- Normal: requires at least one body turn plus meaningful travel.
- Hard: requires navigating past an obstacle or turning a corner.

Tasks should be achievable. Hard should mean interesting, not impossible.

## Distance Goals

Optional. Use when the lesson should teach camera and sensor together.

Examples:

- Identify the target without approaching.
- Approach until the target is clearly framed.
- Approach to within 100cm.
- Approach to within 50cm.
- Approach to within 25cm, only if the operator confirms it is safe.

Distance goals should be measured against the sensor when the target is sensor-readable. If the target is soft, angled, small, or below the sensor line, the operator may need to provide floor truth.

## Agent Prompt

Paste or adapt this for the driver.

```text
You are playing [GAME NAME].

TARGET:
  [operator fills in]

SPACE:
  [open/path/obstacle]

DIFFICULTY:
  [easy/normal/hard]

DISTANCE GOAL:
  [operator fills in]

SAFETY BOUNDARIES:
  [operator fills in]

YOUR GOAL:
  [operator fills in]

Remember: this is practice, not a test. Move, look, read the log, ask for floor truth, and leave useful traces.
```

## Rules Of Play

- Read the observe log before moving.
- Announce your intent before the first move.
- Use camera pan before body movement when orienting.
- Name the uncertainty you are resolving.
- If there is a distance goal, say whether you are trusting camera, sensor, or operator floor truth.
- Ask for floor truth when camera, sensor, and expectation disagree.
- Stop when the operator says stop.

## Round Goals

What the round is trying to accomplish.

## What Counts As A Good Round

A good round may include completing the visible goal, but it should also count:

- clean communication
- useful searching
- safe movement
- learning from correction
- knowing when to ask for help
- leaving a clear trace for the next driver

## Move Budget

Optional. Use only when helpful.

- Easy:
- Normal:
- Hard:

Move budgets should encourage focus without making the round feel punitive.

## Stop Conditions

Always include operator-defined stop conditions. Default examples:

- operator says stop
- stairs, water, cliff, drop-off, or unsafe edge appears
- distance under 20cm unless operator confirms it is safe
- camera unavailable
- frame unchanged after movement
- physical contact suspected

## Debrief Questions

- What did you think the space was at the beginning?
- Which uncertainty did you resolve first?
- What did the camera make look closer or farther than it was?
- What did the log teach you?
- What would you do differently next round?

## Badge Evidence

Which badges could this round support?

- Badge:
- Evidence:
