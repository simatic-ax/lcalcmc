# LCalcMC_typePositioningDetailsVelocity

| Member | Type | Default Value | Description |
|--------|------|---------------|-------------|
| `v0` | `LREAL` | 0.0 | Velocity at t0 (start velocity = 0.0) |
| `v1` | `LREAL` | 0.0 | Velocity at t1 (end of phase where the acceleration is increased = first jerk phase) |
| `v2` | `LREAL` | 0.0 | Velocity at t2 (end of phase where the acceleration is constant) |
| `v3` | `LREAL` | 0.0 | Velocity at t3 (end of phase where the acceleration is decreased = second jerk phase) |
| `v4` | `LREAL` | 0.0 | Velocity at t4 (end of phase where the acceleration is zero = constant velocity phase) |
| `v5` | `LREAL` | 0.0 | Velocity at t5 (end of phase where the deceleration is increased = third jerk phase) |
| `v6` | `LREAL` | 0.0 | Velocity at t6 (end of phase where the deceleration is constant) |
| `v7` | `LREAL` | 0.0 | Velocity at t7 (end of phase where the deceleration is decreased = fourth jerk phase). End velocity = 0.0 |
