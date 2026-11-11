# LCalcMC Library for SIMATIC AX

## Overview

The LCalcMC library provides functions to get detailed information about motion profiles for SIMATIC AX applications.

## Library Structure

The library is organized into the following main components:

### Move Velocity Functions

Functions for calculating velocity changes (`MC_MoveVelocity`, `MC_MoveJog`, `MC_Halt`):

- [`MoveVelocityTime`](./functions/MoveVelocityTime.md): Calculates time needed to reach specified velocity
- [`MoveVelocityDistance`](./functions/MoveVelocityDistance.md): Calculates distance needed to reach specified velocity
- [`MoveVelocityDetails`](./functions/MoveVelocityDetails.md): Calculates detailed motion profile with partial times and distances
- [`MoveVelocityAccelByTime`](./functions/MoveVelocityAccelByTime.md): Calculates required acceleration for specified time
- [`MoveVelocityAccelByDistance`](./functions/MoveVelocityAccelByDistance.md): Calculates required acceleration for specified distance
- [`MoveVelocityJerkByTime`](./functions/MoveVelocityJerkByTime.md): Calculates required jerk for specified time
- [`MoveVelocityJerkByDistance`](./functions/MoveVelocityJerkByDistance.md): Calculates required jerk for specified distance

### Positioning Functions

Functions for calculating positioning movements (`MC_MoveAbsolute`, `MC_MoveRelative`, `MC_MoveSuperimposed`):

- [`PositioningTime`](./functions/PositioningTime.md): Calculates time needed for positioning from standstill to standstill
- [`PositioningDetails`](./functions/PositioningDetails.md): Calculates detailed positioning profile with partial times and distances
- [`PositioningAccel`](./functions/PositioningAccel.md): Calculates required acceleration for positioning in specified time
- [`PositioningJerk`](./functions/PositioningJerk.md): Calculates required jerk for positioning in specified time

### Internal Utility Functions

Additional calculation functions:

- [`TrapezoidalStoppingDetails`](./functions/TrapezoidalStoppingDetails.md): Calculates stopping distance and time with trapezoidal profile
- [`FourthDegreePolyZeros`](./functions/4thDegreePolyZeros.md): Solves 4th degree polynomial equations
- [`LCalcMC.SQRT`](./functions/SQRT.md): Square root calculation function

### Data Types

#### Main Types

- [`typeMoveVelocityDetails`](./types/typeMoveVelocityDetails.md): Complete motion profile details for velocity changes
- [`typePositioningDetails`](./types/typePositioningDetails.md): Complete motion profile details for positioning

#### Internal Sub-Types for Move Velocity Details

- [`typeMoveVelocityDetailsTime`](./types/internalSubTypes/typeMoveVelocityDetailsTime.md): Time values at motion profile kink points
- [`typeMoveVelocityDetailsDistance`](./types/internalSubTypes/typeMoveVelocityDetailsDistance.md): Distance values at motion profile kink points
- [`typeMoveVelocityDetailsVelocity`](./types/internalSubTypes/typeMoveVelocityDetailsVelocity.md): Velocity values at motion profile kink points
- [`typeMoveVelocityDetailsAcceleration`](./types/internalSubTypes/typeMoveVelocityDetailsAcceleration.md): Acceleration values at motion profile kink points
- [`typeMoveVelocityDynamics`](./types/internalSubTypes/typeMoveVelocityDynamics.md): Motion dynamics configuration

#### Internal Sub-Types for Positioning Details

- [`typePositioningDetailsTime`](./types/internalSubTypes/typePositioningDetailsTime.md): Time values at positioning profile kink points
- [`typePositioningDetailsDistance`](./types/internalSubTypes/typePositioningDetailsDistance.md): Distance values at positioning profile kink points
- [`typePositioningDetailsVelocity`](./types/internalSubTypes/typePositioningDetailsVelocity.md): Velocity values at positioning profile kink points
- [`typePositioningDetailsAcceleration`](./types/internalSubTypes/typePositioningDetailsAcceleration.md): Acceleration values at positioning profile kink points

#### Internal Utility Types

- [`type4thDegreePolyZeros`](./types/internalSubTypes/type4thDegreePolyZeros.md): Results from 4th degree polynomial calculation

### Constants

- [`LCalcMC.Constants`](./constants/Constants.md): General library constants
- [`LCalcMC.Status`](./constants/ErrorIDs.md): Error identification constants

## Migration from TIA Portal

This library has been migrated from TIA Portal to SIMATIC AX. The functionality remains the same, but the programming model has been adapted to SIMATIC AX. Key differences include:

- **Namespace**: The library now uses the `Simatic.Ax.LCalcMC` namespace
- **Data types**: The data types have been adapted to SIMATIC AX conventions
- **Error/Status handling**: Error/Status handling has been adapted to use SIMATIC AX error handling patterns
- **Function interfaces**: Function interfaces follow SIMATIC AX naming conventions and parameter patterns
