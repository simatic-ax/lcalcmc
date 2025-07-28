# LCalcMC_4thDegreePolyZeros

## Principle of operation

The function `LCalcMC_4thDegreePolyZeros` calculates the roots (zeros) of a polynomial of 4th degree using the formula ax⁴+bx³+cx²+dx+e = 0. This function is used as a subfunction within other motion control blocks that require solving polynomial equations.

The function returns up to 4 complex roots, each with real and imaginary parts. The status indicates how many real zeros were found.

## Interface

### Input Parameters

| Parameter | Type | Description |
|-----------|------|-------------|
| `coeffA` | `LREAL` | Coefficients of polynomial ax⁴+bx³+cx²+dx+e = 0 |
| `coeffB` | `LREAL` | Coefficients of polynomial ax⁴+bx³+cx²+dx+e = 0 |
| `coeffC` | `LREAL` | Coefficients of polynomial ax⁴+bx³+cx²+dx+e = 0 |
| `coeffD` | `LREAL` | Coefficients of polynomial ax⁴+bx³+cx²+dx+e = 0 |
| `coeffE` | `LREAL` | Coefficients of polynomial ax⁴+bx³+cx²+dx+e = 0 |

### Return Value

| Parameter | Type | Description |
|-----------|------|-------------|
| `LCalcMC_4thDegreePolyZeros` | [`LCalcMC_type4thDegreePolyZeros`](../types/internalSubTypes/LCalcMC_type4thDegreePolyZeros.md) | Structure containing the calculated polynomial zeros and status information |
