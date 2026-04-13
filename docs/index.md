# LCalcMC Library for SIMATIC AX

## Overview

The LCalcMC library provides functions to get detailed information about motion profiles for SIMATIC AX applications.

## Library Structure

The library is organized into the following main components:

### Move Velocity Functions

Functions for calculating velocity changes (`MC_MoveVelocity`, `MC_MoveJog`, `MC_Halt`):

- [`MoveVelocityTime`](./functions/LCalcMC_MoveVelocityTime.md): Calculates time needed to reach specified velocity
- [`MoveVelocityDistance`](./functions/LCalcMC_MoveVelocityDistance.md): Calculates distance needed to reach specified velocity
- [`MoveVelocityDetails`](./functions/LCalcMC_MoveVelocityDetails.md): Calculates detailed motion profile with partial times and distances
- [`MoveVelocityAccelByTime`](./functions/LCalcMC_MoveVelocityAccelByTime.md): Calculates required acceleration for specified time
- [`MoveVelocityAccelByDistance`](./functions/LCalcMC_MoveVelocityAccelByDistance.md): Calculates required acceleration for specified distance
- [`MoveVelocityJerkByTime`](./functions/LCalcMC_MoveVelocityJerkByTime.md): Calculates required jerk for specified time
- [`MoveVelocityJerkByDistance`](./functions/LCalcMC_MoveVelocityJerkByDistance.md): Calculates required jerk for specified distance

### Positioning Functions

Functions for calculating positioning movements (`MC_MoveAbsolute`, `MC_MoveRelative`, `MC_MoveSuperimposed`):

- [`PositioningTime`](./functions/LCalcMC_PositioningTime.md): Calculates time needed for positioning from standstill to standstill
- [`PositioningDetails`](./functions/LCalcMC_PositioningDetails.md): Calculates detailed positioning profile with partial times and distances
- [`PositioningAccel`](./functions/LCalcMC_PositioningAccel.md): Calculates required acceleration for positioning in specified time
- [`PositioningJerk`](./functions/LCalcMC_PositioningJerk.md): Calculates required jerk for positioning in specified time

### Internal Utility Functions

Additional calculation functions:

- [`TrapezoidalStoppingDetails`](./functions/LCalcMC_TrapezoidalStoppingDetails.md): Calculates stopping distance and time with trapezoidal profile
- [`FourthDegreePolyZeros`](./functions/LCalcMC_4thDegreePolyZeros.md): Solves 4th degree polynomial equations
- [`LCalcMC.SQRT`](./functions/LCalcMC_SQRT.md): Square root calculation function

### Data Types

#### Main Types

- [`typeMoveVelocityDetails`](./types/LCalcMC_typeMoveVelocityDetails.md): Complete motion profile details for velocity changes
- [`typePositioningDetails`](./types/LCalcMC_typePositioningDetails.md): Complete motion profile details for positioning

#### Internal Sub-Types for Move Velocity Details

- [`typeMoveVelocityDetailsTime`](./types/internalSubTypes/LCalcMC_typeMoveVelocityDetailsTime.md): Time values at motion profile kink points
- [`typeMoveVelocityDetailsDistance`](./types/internalSubTypes/LCalcMC_typeMoveVelocityDetailsDistance.md): Distance values at motion profile kink points
- [`typeMoveVelocityDetailsVelocity`](./types/internalSubTypes/LCalcMC_typeMoveVelocityDetailsVelocity.md): Velocity values at motion profile kink points
- [`typeMoveVelocityDetailsAcceleration`](./types/internalSubTypes/LCalcMC_typeMoveVelocityDetailsAcceleration.md): Acceleration values at motion profile kink points
- [`typeMoveVelocityDynamics`](./types/internalSubTypes/LCalcMC_typeMoveVelocityDynamics.md): Motion dynamics configuration

#### Internal Sub-Types for Positioning Details

- [`typePositioningDetailsTime`](./types/internalSubTypes/LCalcMC_typePositioningDetailsTime.md): Time values at positioning profile kink points
- [`typePositioningDetailsDistance`](./types/internalSubTypes/LCalcMC_typePositioningDetailsDistance.md): Distance values at positioning profile kink points
- [`typePositioningDetailsVelocity`](./types/internalSubTypes/LCalcMC_typePositioningDetailsVelocity.md): Velocity values at positioning profile kink points
- [`typePositioningDetailsAcceleration`](./types/internalSubTypes/LCalcMC_typePositioningDetailsAcceleration.md): Acceleration values at positioning profile kink points

#### Internal Utility Types

- [`type4thDegreePolyZeros`](./types/internalSubTypes/LCalcMC_type4thDegreePolyZeros.md): Results from 4th degree polynomial calculation

### Constants

- [`LCalcMC.Constants`](./constants/LCalcMC_Constants.md): General library constants
- [`LCalcMC.Status`](./constants/LCalcMC_ErrorIDs.md): Error identification constants

## Migration from TIA Portal

This library has been migrated from TIA Portal to SIMATIC AX. The functionality remains the same, but the programming model has been adapted to SIMATIC AX. Key differences include:

- **Namespace**: The library now uses the `Simatic.Ax.LCalcMC` namespace
- **Data types**: The data types have been adapted to SIMATIC AX conventions
- **Error/Status handling**: Error/Status handling has been adapted to use SIMATIC AX error handling patterns
- **Function interfaces**: Function interfaces follow SIMATIC AX naming conventions and parameter patterns
