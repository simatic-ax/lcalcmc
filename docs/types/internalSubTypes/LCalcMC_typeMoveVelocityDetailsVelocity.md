# LCalcMC_typeMoveVelocityDetailsVelocity

| Member | Type | Default Value | Description |
|--------|------|---------------|-------------|
| `v0` | `LREAL` | 0.0 | Velocity at t0 (input 'startVelocity') |
| `v1` | `LREAL` | 0.0 | Velocity at t1 (end of phase where the acceleration/deceleration is increased = first jerk phase) |
| `v2` | `LREAL` | 0.0 | Velocity at t2 (end of phase where the acceleration/deceleration is constant) |
| `v3` | `LREAL` | 0.0 | Velocity at t3 (end of phase where the acceleration/deceleration is decreased = second jerk phase) |
| `v4` | `LREAL` | 0.0 | Velocity at t4 (end of phase where the deceleration/acceleration is increased = third jerk phase). Note: the corresponding phase only exists if a reversal of the velocity takes place |
| `v5` | `LREAL` | 0.0 | Velocity at t5 (end of phase where the deceleration/acceleration is constant). Note: the corresponding phase only exists if a reversal of the velocity takes place |
| `v6` | `LREAL` | 0.0 | Velocity at t6 (end of phase where the deceleration/acceleration is decreased = fourth jerk phase). Note: the corresponding phase only exists if a reversal of the velocity takes place |
