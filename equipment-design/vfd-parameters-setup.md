# VFD Parameter Setup Checklist

Basic configuration checklist for commissioning a new VFD.

Always consult the **manufacturer manual**, but these parameters exist on nearly all drives.

---

# 1. Motor Nameplate Parameters

Enter motor data exactly from the motor nameplate.

Checklist:

- motor rated voltage
- motor rated current
- motor rated frequency
- motor rated RPM
- motor rated power (HP or kW)

Example:

```
Motor Voltage: 230V
Motor Current: 6.5A
Motor Frequency: 60Hz
Motor Speed: 1725 RPM
Motor Power: 2 HP
```

This allows the VFD to calculate proper current limits.

---

# 2. Maximum Frequency

Maximum motor speed limit.

Typical values:

```
Standard motors: 60 Hz
Light overspeed: 75–90 Hz
```

Avoid extreme overspeed unless the motor is rated for it.

---

# 3. Minimum Frequency

Prevents running motor too slowly.

Typical setting:

```
5–10 Hz
```

Below this range cooling becomes poor.

---

# 4. Acceleration Time

Time to ramp from 0 → full speed.

Typical value:

```
2–5 seconds
```

Heavy machines may require longer ramp time.

---

# 5. Deceleration Time

Time to ramp down to stop.

Typical value:

```
3–10 seconds
```

Short deceleration can cause **overvoltage faults**.

---

# 6. Control Mode

Choose how the VFD receives commands.

Options usually include:

```
Keypad control
External buttons
0-10V speed control
Serial communication
```

Typical shop configuration:

```
Start / Stop buttons
Speed potentiometer
```

---

# 7. Direction Control

Enable forward / reverse if needed.

```
Forward only (recommended for most machines)
Forward / reverse (for lathes, mills, etc.)
```

---

# 8. Current Limit

Protects motor from overload.

Typical setting:

```
110–120% of motor rated current
```

Example:

```
Motor rated current: 6.5A
Current limit: 7.2A
```

---

# 9. Carrier Frequency

Controls switching noise.

Lower values:

- cooler VFD
- more motor noise

Higher values:

- quieter motor
- slightly more VFD heating

Typical range:

```
4–8 kHz
```

---

# 10. Motor Auto-Tune (if available)

Many VFDs include an **auto-tune function**.

Procedure:

1. Disconnect motor load if possible
2. Run auto-tune procedure
3. Allow VFD to measure motor parameters

Benefits:

- smoother control
- improved torque
- better efficiency

---

# 11. Safety Limits

Configure protective limits.

Recommended checks:

- overcurrent trip
- overvoltage protection
- undervoltage protection
- stall protection

These are usually enabled by default.

---

# 12. Test Run Procedure

Before running the machine under load:

1. Start motor at low speed
2. Verify rotation direction
3. Increase speed slowly
4. Monitor current draw
5. Check for vibration or noise

If rotation is incorrect:

```
Swap any two motor output wires
```

---

# 13. Final Checks

Before full operation:

- verify cooling fans working
- confirm airflow
- check enclosure temperature
- inspect wiring connections

---

# Summary

Minimum setup steps:

```
Enter motor nameplate
Set max frequency
Set accel/decel times
Configure control inputs
Verify rotation
```

Once configured properly, most VFD systems run reliably for many years.
