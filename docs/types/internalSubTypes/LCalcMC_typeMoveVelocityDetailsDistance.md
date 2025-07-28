# LCalcMC_typeMoveVelocityDetailsDistance

| Member | Type | Default Value | Description |
|--------|------|---------------|-------------|
| `d0` | `LREAL` | 0.0 | Moved distance at t0 (start distance = 0.0) |
| `d1` | `LREAL` | 0.0 | Moved distance at t1 (end of phase where the acceleration/deceleration is increased = first jerk phase) |
| `d2` | `LREAL` | 0.0 | Moved distance at t2 (end of phase where the acceleration/deceleration is constant) |
| `d3` | `LREAL` | 0.0 | Moved distance at t3 (end of phase where the acceleration/deceleration is decreased = second jerk phase) |
| `d4` | `LREAL` | 0.0 | Moved distance at t4 (end of phase where the deceleration/acceleration is increased = third jerk phase). Note: the corresponding phase only exists if a reversal of the velocity takes place |
| `d5` | `LREAL` | 0.0 | Moved distance at t5 (end of phase where the deceleration/acceleration is constant). Note: the corresponding phase only exists if a reversal of the velocity takes place |
| `d6` | `LREAL` | 0.0 | Moved distance at t6 (end of phase where the deceleration/acceleration is decreased = fourth jerk phase). Note: the corresponding phase only exists if a reversal of the velocity takes place. The value of d6 corresponds to the total distance in any case |
