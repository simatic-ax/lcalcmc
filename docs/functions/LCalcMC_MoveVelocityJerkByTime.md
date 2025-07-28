# LCalcMC_MoveVelocityJerkByTime

## Principle of operation

The function `LCalcMC_MoveVelocityJerkByTime` calculates the jerk needed to reach the specified velocity from starting dynamics (velocity and acceleration at start) by defining a time in which the specified velocity has to be reached. The dynamic values are taken into account (acceleration, deceleration).

## Interface

### Input Parameters

| Parameter | Type | Description |
|-----------|------|-------------|
| `_time` | `LREAL` | Time between start and end of motion command |
| `startVelocity` | `LREAL` | Velocity setpoint at start of motion command |
| `startAcceleration` | `LREAL` | Acceleration setpoint at start of motion command |
| `velocity` | `LREAL` | Velocity setpoint at end of motion command |
| `acceleration` | `LREAL` | Acceleration of motion command |
| `deceleration` | `LREAL` | Deceleration of motion command |

### Output Parameters

| Parameter | Type | Description |
|-----------|------|-------------|
| `jerk` | `LREAL` | Calculated jerk of motion command |

### Return Value

| Parameter | Type | Description |
|-----------|------|-------------|
| `LCalcMC_MoveVelocityJerkByTime` | `WORD` | Status of the function; WORD#16#0000: Calculation finished successfully <br/> WORD#16#8000 - WORD#16#FFFF: Error identification |

The error codes are defined in [`LCalcMC_ErrorIDs`](../constants/LCalcMC_ErrorIDs.md).
