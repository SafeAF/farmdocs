# VFD Enclosure Build Guide

Practical guide for building a cooled VFD enclosure for a **240 V single-phase input → 3-phase motor** system.

## Assumptions

- Metal enclosure
- Cabinet cooling fans
- Shop environment (dust present)
- Basic electrical safety knowledge

If any of these assumptions are wrong, adjust the design before building.

---

# 1. Enclosure Selection

## Requirements

- Metal enclosure (steel preferred)
- Grounded door
- Internal mounting plate
- Adequate vertical space for VFD cooling
- Ability to mount vents and fans

## Rule of Thumb

Leave at least **3–4 inches of clearance above and below the VFD heat sink**.

Most VFDs rely on **vertical convection cooling**.

---

# 2. Layout Planning

Plan the layout **before drilling any holes**.

Key design goal:

Separate **power wiring** from **control wiring**.

## Recommended Layout

TOP  
exhaust fans

VFD

line power in    motor output out

filtered intake

BOTTOM

## Design Rules

- Airflow should move **bottom → top**
- Motor cables should exit away from control wiring
- Leave space for service access

---

# 3. Components Checklist

## Electrical

- VFD
- Main disconnect switch or breaker
- Grounding lug
- DIN rail (optional)
- Terminal blocks for motor wiring
- Cable glands or strain reliefs
- Wire ferrules (recommended)

## Cooling

- 80 mm cabinet fans
- Fan guards
- Intake vent grille
- Filter material

## Protection

- Input fuse or breaker
- EMI / RFI line filter (optional)
- Surge suppressor or MOV (optional)

---

# 4. Grounding

Proper grounding is critical.

## Grounding Checklist

- enclosure bonded to ground
- VFD ground terminal bonded
- motor frame grounded
- enclosure door bonded with ground strap
- cable shields bonded (if using shielded motor cable)

Use **green or green/yellow wire only** for grounding.

Never fuse the ground conductor.

---

# 5. Airflow System

Goal: **filtered intake + exhaust fan cooling**

## Recommended Configuration

Bottom panel  
filtered intake vent

Top panel  
1–2 exhaust fans

## Airflow Path

filter → across VFD heat sink → exhaust fan

## Avoid

- blowing dust directly into the enclosure
- recirculating air inside a sealed enclosure
- mounting the fan blowing directly at electronics

---

# 6. Cable Routing

Separate wiring into three zones.

## Input Power

240 V supply → disconnect → VFD input

## Motor Output

VFD → motor cable

## Control Wiring

- start / stop
- speed potentiometer
- forward / reverse

Rule:  
Motor output cables must **not run alongside control wiring**.

VFD output produces electrical noise.

---

# 7. Input Power Wiring

Typical wiring configuration:

L1 → disconnect → VFD R  
L2 → disconnect → VFD S  
Ground → VFD PE

## Important Notes

- Neutral is **not required**
- Ground must never be fused
- Avoid running VFDs through GFCI unless necessary

---

# 8. Motor Wiring

Typical output terminals:

VFD U → motor T1  
VFD V → motor T2  
VFD W → motor T3  
Ground → motor frame

## Best Practices

- Use VFD-rated motor cable if possible
- Keep motor cable short
- Route separately from control wiring

---

# 9. Fan Wiring

Fans rated for **220–240 V AC** can be wired directly across the supply.

Example wiring:

L1 → fan  
L2 → fan

Connect fans **after the disconnect but before the VFD input**.

This allows the fan to run whenever the enclosure is powered.

---

# 10. Control Interface (Optional)

Many installations include:

- Start button
- Stop button
- Speed potentiometer
- Forward / reverse switch

These connect to the **VFD control terminals**.

Control wiring must be separated from motor cables.

---

# 11. EMI / Electrical Noise Control

VFDs generate electrical noise.

Recommended practices:

- Keep motor cable short
- Use shielded cable for long runs
- Maintain good grounding
- Use metal enclosure

Optional improvement:

Install an **EMI filter between mains and VFD input**.

---

# 12. Initial Power-Up Checklist

Before energizing:

- all grounds connected
- no exposed copper strands
- motor wiring verified
- fans spin freely
- airflow path clear
- VFD mounted vertically
- cables secured

First power-up should be done **without running the motor**.

---

# 13. First Run Procedure

1. Power the enclosure
2. Verify fan operation
3. Program VFD motor parameters
4. Run motor at low frequency
5. Verify rotation direction
6. Monitor current and temperature

If motor rotation is reversed:

Swap **any two motor output wires**.

---

# 14. Long-Term Maintenance

- Clean intake filter periodically
- Vacuum enclosure annually
- Check fan operation
- Inspect wiring connections

Dust buildup and poor cooling are common causes of VFD failure.

---

# 15. Common Mistakes

Avoid the following:

- mounting the VFD horizontally
- no enclosure ventilation
- motor cables routed with control wiring
- poor grounding
- plastic enclosures
- blowing dusty air directly into the enclosure

---

# Summary

A reliable VFD enclosure should include:

- grounded metal enclosure
- proper cable routing
- filtered airflow
- exhaust cooling fans
- solid grounding

When built correctly, a VFD enclosure can run **for many years in a shop environment** with minimal maintenance.
