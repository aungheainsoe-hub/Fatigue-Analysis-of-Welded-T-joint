# Fatigue Analysis of a Welded T-Joint

Fatigue assessment of a welded T-joint comparing three stress-based approaches
from the IIW recommendations: structural (hot-spot) stress, through-thickness
structural stress at the weld toe, and effective notch stress.

## Overview
Welded joints fail by fatigue at the weld toe long before the base material does,
so the stress method you use to assess them matters. This project evaluates the
same welded T-joint with three established approaches and compares the fatigue
results they give.

## Methods compared
- **Hot-spot / structural stress (HS)** — structural stress at the weld toe found by
  surface-stress extrapolation to the toe, assessed against the hot-spot FAT class.
- **Through-thickness at weld toe (TTWT)** — structural stress obtained by linearising
  the through-thickness stress distribution at the weld toe into membrane + bending.
- **Effective notch stress (ENS)** — the weld toe/root modelled with a 1 mm reference
  radius to capture the peak notch stress, assessed against the ENS FAT class.

## Tools & methods
- Finite element analysis (Ansys)
- Mesh refinement at the weld toe (fine mesh + 1 mm reference notch for ENS)
- Stress extraction, structural-stress linearisation, and fatigue assessment to
  IIW recommendations (FAT classes / S-N curves)

## What was done
- Built an FE model of the welded T-joint
- Extracted weld-toe stresses and applied each of the three approaches
- Derived the relevant fatigue stress for each method and compared against the
  corresponding FAT class to estimate fatigue strength / life

## Repository contents
- `Exercise 4/` — FE model files, results, and working
- `Exercise4.zip` — packaged project files
