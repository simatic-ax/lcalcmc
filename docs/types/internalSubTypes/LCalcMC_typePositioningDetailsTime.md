# LCalcMC_typePositioningDetailsTime

| Member | Type | Default Value | Description |
|--------|------|---------------|-------------|
| `t0` | `LREAL` | 0.0 | Elapsed time at t0 (start time = 0.0) |
| `t1` | `LREAL` | 0.0 | Elapsed time at t1 (end of phase where the acceleration is increased = first jerk phase) |
| `t2` | `LREAL` | 0.0 | Elapsed time at t2 (end of phase where the acceleration is constant) |
| `t3` | `LREAL` | 0.0 | Elapsed time at t3 (end of phase where the acceleration is decreased = second jerk phase) |
| `t4` | `LREAL` | 0.0 | Elapsed time at t4 (end of phase where the acceleration is zero = constant velocity phase) |
| `t5` | `LREAL` | 0.0 | Elapsed time at t5 (end of phase where the deceleration is increased = third jerk phase) |
| `t6` | `LREAL` | 0.0 | Elapsed time at t6 (end of phase where the deceleration is constant) |
| `t7` | `LREAL` | 0.0 | Elapsed time at t7 (end of phase where the deceleration is decreased = fourth jerk phase). Note: the value of t7 corresponds to the total time in any case |
