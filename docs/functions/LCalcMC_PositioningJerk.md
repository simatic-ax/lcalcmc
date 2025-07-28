# LCalcMC_PositioningJerk

## Principle of operation

The function `LCalcMC_PositioningJerk` calculates the jerk that is needed to move a specified distance in a given time with a positioning command from standstill to standstill. The dynamic values are taken into account (velocity, acceleration, deceleration).

## Interface

### Input Parameters

| Parameter | Type | Description |
|-----------|------|-------------|
| `_time` | `LREAL` | Time between start and end of motion command |
| `distance` | `LREAL` | Distance between start and end of motion command |
| `velocity` | `LREAL` | Velocity of motion command |
| `acceleration` | `LREAL` | Acceleration of motion command |
| `deceleration` | `LREAL` | Deceleration of motion command |

### Output Parameters

| Parameter | Type | Description |
|-----------|------|-------------|
| `jerk` | `LREAL` | Calculated jerk of motion command |

### Return Value

| Parameter | Type | Description |
|-----------|------|-------------|
| `LCalcMC_PositioningJerk` | `WORD` | Status of the function; WORD#16#0000: Calculation finished successfully <br/> WORD#16#8000 - WORD#16#FFFF: Error identification |

The error codes are defined in [`LCalcMC_ErrorIDs`](../constants/LCalcMC_ErrorIDs.md).
