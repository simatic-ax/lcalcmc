# LCalcMC_Constants

## Description

The `LCalcMC_Constants` type defines constants used for tolerance calculations in the LCalcMC library. These constants provide numerical tolerance values for motion control calculations to handle floating-point precision issues.

## Constants

| Constant | Value | Description |
|----------|-------|-------------|
| `LCALCMC_MIN_JERK_TOLERANCE` | 1.0E-05 | Tolerance value for minimum jerk calculation at comparisons in configured unit |

## Usage

These constants are used internally by the motion control functions to provide numerical stability when comparing calculated values with theoretical limits. The tolerance helps to avoid issues with floating-point arithmetic precision in motion control calculations.
