# LCalcMC_TrapezoidalStoppingDetails

## Principle of operation

The function `LCalcMC_TrapezoidalStoppingDetails` calculates the distance needed to stop the axis with a trapezoidal profile. The dynamic values are taken into account (only parameter deceleration is required).

## Interface

### Input Parameters

| Parameter | Type | Description |
|-----------|------|-------------|
| `startVelocity` | `LREAL` | Velocity setpoint at start of motion command |
| `deceleration` | `LREAL` | Deceleration of motion command |

### Output Parameters

| Parameter | Type | Description |
|-----------|------|-------------|
| `distance` | `LREAL` | Calculated distance moved until axis is in standstill |
| `_time` | `LREAL` | Calculated time for stopping |

### Return Value

| Parameter | Type | Description |
|-----------|------|-------------|
| `LCalcMC_TrapezoidalStoppingDetails` | `WORD` | Status of the function; WORD#16#0000: Calculation finished successfully <br/> WORD#16#8000 - WORD#16#FFFF: Error identification |

The error codes are defined in [`LCalcMC_ErrorIDs`](../constants/LCalcMC_ErrorIDs.md).
