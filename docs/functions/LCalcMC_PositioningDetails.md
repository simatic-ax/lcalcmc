# LCalcMC_PositioningDetails

## Principle of operation

The function `LCalcMC_PositioningDetails` calculates the total time and total distance as well as part times, part distances, velocities and accelerations at the kink points of the acceleration. The dynamic values are taken into account (velocity, acceleration, deceleration, jerk).

This example shows a positioning movement where the limits for acceleration, deceleration and velocity are maintained. In this case, all seven time phases are greater than 0.0, where time t0 is always 0.0.

![InflectionPoint](../assets/images/example_pos_command.png)

## Interface

### Input Parameters

| Parameter | Type | Description |
|-----------|------|-------------|
| `distance` | `LREAL` | Distance between start and end of motion command |
| `velocity` | `LREAL` | Velocity of motion command |
| `acceleration` | `LREAL` | Acceleration of motion command |
| `deceleration` | `LREAL` | Deceleration of motion command |
| `jerk` | `LREAL` | Jerk of motion command (Value:=0.0: Trapezoid velocity profile) |

### Output Parameters

| Parameter | Type | Description |
|-----------|------|-------------|
| `positioningDetails` | [`LCalcMC_typePositioningDetails`](../types/LCalcMC_typePositioningDetails.md) | Calculated times, distances, velocities and accelerations between start and end of motion command |

### Return Value

| Parameter | Type | Description |
|-----------|------|-------------|
| `LCalcMC_PositioningDetails` | `WORD` | Status of the function; WORD#16#0000: Calculation finished successfully <br/> WORD#16#8000 - WORD#16#FFFF: Error identification |

The error codes are defined in [`LCalcMC_ErrorIDs`](../constants/LCalcMC_ErrorIDs.md).
