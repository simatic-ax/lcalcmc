# LCalcMC_MoveVelocityDistance

## Principle of operation

The function `LCalcMC_MoveVelocityDistance` calculates the distance needed to reach the specified velocity from starting dynamics (velocity and acceleration at start). The dynamic values are taken into account (acceleration, deceleration, jerk). The direction of the movement is signalized by the sign.

**_NOTE:_** The function can also be used to calculate the distance for a jerk limited stop.

## Interface

### Input Parameters

| Parameter | Type | Description |
|-----------|------|-------------|
| `startVelocity` | `LREAL` | Velocity setpoint at start of motion command |
| `startAcceleration` | `LREAL` | Acceleration setpoint at start of motion command |
| `velocity` | `LREAL` | Velocity setpoint at end of motion command |
| `acceleration` | `LREAL` | Acceleration of motion command |
| `deceleration` | `LREAL` | Deceleration of motion command |
| `jerk` | `LREAL` | Jerk of motion command (Value = 0.0: Trapezoid velocity profile) |

### Output Parameters

| Parameter | Type | Description |
|-----------|------|-------------|
| `distance` | `LREAL` | Calculated distance moved between start and end of motion command |

### Return Value

| Parameter | Type | Description |
|-----------|------|-------------|
| `LCalcMC_MoveVelocityDistance` | `WORD` | Status of the function; WORD#16#0000: Calculation finished successfully <br/> WORD#16#8000 - WORD#16#FFFF: Error identification |

The error codes are defined in [`LCalcMC_ErrorIDs`](../constants/LCalcMC_ErrorIDs.md).
