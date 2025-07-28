# LCalcMC_typePositioningDetailsDistance

| Member | Type | Default Value | Description |
|--------|------|---------------|-------------|
| `d0` | `LREAL` | 0.0 | Moved distance at t0 (start distance = 0.0) |
| `d1` | `LREAL` | 0.0 | Moved distance at t1 (end of phase where the acceleration is increased = first jerk phase) |
| `d2` | `LREAL` | 0.0 | Moved distance at t2 (end of phase where the acceleration is constant) |
| `d3` | `LREAL` | 0.0 | Moved distance at t3 (end of phase where the acceleration is decreased = second jerk phase) |
| `d4` | `LREAL` | 0.0 | Moved distance at t4 (end of phase where the acceleration is zero = constant velocity phase) |
| `d5` | `LREAL` | 0.0 | Moved distance at t5 (end of phase where the deceleration is increased = third jerk phase) |
| `d6` | `LREAL` | 0.0 | Moved distance at t6 (end of phase where the deceleration is constant) |
| `d7` | `LREAL` | 0.0 | Moved distance at t7 (end of phase where the deceleration is decreased = fourth jerk phase). Note: the value of d7 corresponds to the total distance in any case |
