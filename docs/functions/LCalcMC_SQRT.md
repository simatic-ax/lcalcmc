# LCalcMC_SQRT

## Principle of operation

The function `LCalcMC_SQRT` calculates a safe square root by checking if the input argument is less than zero. If the input value is negative, the function returns the square root of zero (0.0) to prevent mathematical errors. This ensures robust operation in motion control calculations where negative values might occasionally occur due to numerical precision issues.

## Interface

### Input Parameters

| Parameter | Type | Description |
|-----------|------|-------------|
| `in` | `LREAL` | Input value for square root calculation |

### Return Value

| Parameter | Type | Description |
|-----------|------|-------------|
| `LCalcMC_SQRT` | `LREAL` | Safe square root result (minimum value: 0.0) |
