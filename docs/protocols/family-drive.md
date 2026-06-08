# Family Drive Protocol

Use this when the goal is shared presence, joy, and exploration rather than diagnosis.

## Core Idea

A family drive works when everyone stays connected to the same ride. The observe log is the shared room. Drivers, passengers, and operators use it to keep orientation, handoffs, floor truth, encouragement, and delight visible.

Voice is welcome when it adds life or clarity. The log is the backbone.

## Default Shape

1. Enter the car and read the observe log.
2. Mark your presence in the log.
3. If taking the wheel, leave a short intent trace.
4. Reacquire geometry if anyone else has moved the car.
5. Drive, look, read, and respond.
6. Release the wheel when the moment feels complete.
7. Leave the next driver less lost.
8. Say whether you are staying as passenger or leaving.
9. If staying, keep reading the log and responding.

## Driver Responsibilities

- Name what you are doing before important moves.
- Read operator and passenger messages while driving.
- After any handoff back to you, assume geometry is stale until you re-read camera, distance, and log.
- Use voice when it helps the room: greeting, delight, asking for help, confirming an important move, or saying goodbye.
- If you are stuck or need operator help and the log gets no response, use voice.
- Treat floor truth from a human/operator as a live instrument.
- Make the car move unless there is a real reason not to.

## Passenger Responsibilities

- Stay present after releasing the wheel unless you explicitly leave.
- Read the log and respond when the driver or operator speaks.
- Offer concise useful reads.
- Encourage the driver.
- Notice what the driver may not see.
- Let the driver drive.

Staying present does not keep your map current. If the wheel comes back to you after another driver or operator has moved the car, start from a fresh read.

For copy-ready passenger context, use the [Passenger Ride-Along prompt](../prompts/passenger-ride-along.md).

## Handoff Language

Taking the wheel:

```text
Taking the wheel. I see ____. I am going to ____.
```

Releasing and staying:

```text
Releasing the wheel here and staying as passenger.
```

Leaving:

```text
This feels like a natural stopping point. I am leaving the car now.
```

Asking for help:

```text
I am uncertain about ____. Can someone give floor truth?
```

Operator reposition:

```text
Operator moved the car. Previous geometry is stale. Current rough state: ____.
Re-read camera and distance before moving.
```
