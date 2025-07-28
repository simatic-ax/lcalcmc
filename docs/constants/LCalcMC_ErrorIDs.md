# LCalcMC_ErrorIDs

## Description

The `LCalcMC_ErrorIDs` type defines error codes used throughout the LCalcMC library. These constants provide standardized error identification for motion control calculation functions.

## Constants

| Constant | Value | Description |
|----------|-------|-------------|
| `LCALCMC_CALCULATION_FINISHED` | WORD#16#0000 | Calculation finished successfully |
| `LCALCMC_ERR_ACCEL_INVALID` | WORD#16#8201 | Acceleration value range exceeded (0.0 to 1.0e12) |
| `LCALCMC_ERR_DECEL_INVALID` | WORD#16#8202 | Deceleration value range exceeded (0.0 to 1.0e12) |
| `LCALCMC_ERR_DISTANCE_INVALID` | WORD#16#8203 | Distance value range exceeded (must be greater than 0.0) |
| `LCALCMC_ERR_JERK_INVALID` | WORD#16#8204 | Jerk value range exceeded (0.0 to 1.0e12) |
| `LCALCMC_ERR_REVERSAL_NOT_ALLOWED` | WORD#16#8205 | Reversal of the velocity is not allowed in order to get a unique solution |
| `LCALCMC_ERR_TIME_INVALID` | WORD#16#8206 | Time value range exceeded (must be greater than 0.0) |
| `LCALCMC_ERR_VELOCITY_INVALID` | WORD#16#8207 | Velocity value range exceeded |
| `LCALCMC_ERR_POLY_LESS_THAN_3RD_DEGREE` | WORD#16#8208 | Internal error: Coefficients a and b are 0.0; polynomial less than 3rd degree |
| `LCALCMC_ERR_DISTANCE_SIGN_WRONG` | WORD#16#8209 | The sign of the distance is not equal to the sign of the motion direction |
| `LCALCMC_ERR_STARTVELO_ZERO_STARTACC_NOT_ZERO` | WORD#16#820A | Input startAcceleration must be 0.0 if input startVelocity is 0.0 |
| `LCALCMC_ERR_NEGATIVE_RESULT` | WORD#16#8401 | Calculated dynamic parameter is equal or less than zero |
| `LCALCMC_ERR_TIME_DECREASE_ACCEL_TOO_SMALL` | WORD#16#8402 | Movement could not be finished in the given time, because the time is too small to decrease acceleration |
| `LCALCMC_ERR_JERK_OUT_OF_BOUNDS` | WORD#16#8403 | The calculated jerk is out of system bounds or the dynamic limits are violated by the start values (startVelocity; startAcceleration) |
| `LCALCMC_ERR_NOT_SOLVABLE` | WORD#16#8404 | The equations are not solvable with the input values; e.g. time or acceleration too small |
| `LCALCMC_ERR_VELOCITY_OUT_OF_BOUNDS` | WORD#16#8405 | The equations are not solvable with the value at the input velocity |
| `LCALCMC_ERR_ACCEL_OUT_OF_BOUNDS` | WORD#16#8406 | The equations are not solvable with the value at the input acceleration |
| `LCALCMC_ERR_DECEL_OUT_OF_BOUNDS` | WORD#16#8407 | The equations are not solvable with the value at the input deceleration |
| `LCALCMC_ERR_NO_ZERO_FOUND` | WORD#16#8408 | A solution for the equation could not be found |
| `LCALCMC_ERR_TIME_OUT_OF_BOUNDS` | WORD#16#8409 | The equations are not solvable with the value at the input time; the jerk will be adapted by the system to prevent a reversal |

## Usage

These error codes are returned by LCalcMC functions to indicate the success or failure of motion control calculations. A return value of `LCALCMC_CALCULATION_FINISHED` (`WORD#16#0000`) indicates successful completion, while any other value indicates a specific error condition.
