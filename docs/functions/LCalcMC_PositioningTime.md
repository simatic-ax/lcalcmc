# LCalcMC_PositioningTime

## Principle of operation

The function `LCalcMC_PositioningTime` calculates the time needed to move a specified distance with a positioning command from standstill to standstill. The dynamic values are taken into account (velocity, acceleration, deceleration, jerk).

## Interface

### Input Parameters

| Parameter | Type | Description |
|-----------|------|-------------|
| `distance` | `LREAL` | Distance between start and end of motion command |
| `velocity` | `LREAL` | Velocity of motion command |
| `acceleration` | `LREAL` | Acceleration of motion command |
| `deceleration` | `LREAL` | Deceleration of motion command |
| `jerk` | `LREAL` | Jerk of motion command (Value = 0.0: Trapezoid velocity profile) |

### Output Parameters

| Parameter | Type | Description |
|-----------|------|-------------|
| `_time` | `LREAL` | Calculated time between start and end of motion command |

### Return Value

| Parameter | Type | Description |
|-----------|------|-------------|
| `LCalcMC_PositioningTime` | `WORD` | Status of the function; WORD#16#0000: Calculation finished successfully <br/> WORD#16#8000 - WORD#16#FFFF: Error identification |

The error codes are defined in [`LCalcMC_ErrorIDs`](../constants/LCalcMC_ErrorIDs.md).
