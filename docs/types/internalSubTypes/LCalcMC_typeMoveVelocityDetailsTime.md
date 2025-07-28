# LCalcMC_typeMoveVelocityDetailsTime

| Member | Type | Default Value | Description |
|--------|------|---------------|-------------|
| `t0` | `LREAL` | 0.0 | Elapsed time at t0 (start time = 0.0) |
| `t1` | `LREAL` | 0.0 | Elapsed time at t1 (end of phase where the acceleration/deceleration is increased = first jerk phase) |
| `t2` | `LREAL` | 0.0 | Elapsed time at t2 (end of phase where the acceleration/deceleration is constant) |
| `t3` | `LREAL` | 0.0 | Elapsed time at t3 (end of phase where the acceleration/deceleration is decreased = second jerk phase) |
| `t4` | `LREAL` | 0.0 | Elapsed time at t4 (end of phase where the deceleration/acceleration is increased = third jerk phase). Note: the corresponding phase only exists if a reversal of the velocity takes place |
| `t5` | `LREAL` | 0.0 | Elapsed time at t5 (end of phase where the deceleration/acceleration is constant). Note: the corresponding phase only exists if a reversal of the velocity takes place |
| `t6` | `LREAL` | 0.0 | Elapsed time at t6 (end of phase where the deceleration/acceleration is decreased = fourth jerk phase). Note: the corresponding phase only exists if a reversal of the velocity takes place. The value of t6 corresponds to the total time in any case |
