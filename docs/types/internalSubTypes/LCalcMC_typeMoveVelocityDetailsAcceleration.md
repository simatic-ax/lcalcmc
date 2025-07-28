# LCalcMC_typeMoveVelocityDetailsAcceleration

| Member | Type | Default Value | Description |
|--------|------|---------------|-------------|
| `a0` | `LREAL` | 0.0 | Acceleration at t0 (input 'startAcceleration') |
| `a1` | `LREAL` | 0.0 | Acceleration at t1 (end of phase where the acceleration/deceleration is increased = first jerk phase) |
| `a2` | `LREAL` | 0.0 | Acceleration at t2 (end of phase where the acceleration/deceleration is constant) |
| `a3` | `LREAL` | 0.0 | Acceleration at t3 (end of phase where the acceleration/deceleration is decreased = second jerk phase) |
| `a4` | `LREAL` | 0.0 | Acceleration at t4 (end of phase where the deceleration/acceleration is increased = third jerk phase). Note: the corresponding phase only exists if a reversal of the velocity takes place |
| `a5` | `LREAL` | 0.0 | Acceleration at t5 (end of phase where the deceleration/acceleration is constant). Note: the corresponding phase only exists if a reversal of the velocity takes place |
| `a6` | `LREAL` | 0.0 | Acceleration at t6 (end of phase where the deceleration/acceleration is decreased = fourth jerk phase). Note: the corresponding phase only exists if a reversal of the velocity takes place |
