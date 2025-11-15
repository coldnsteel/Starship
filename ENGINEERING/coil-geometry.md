# Coil Geometry & Field Delivery

## Overview [PILOT]
Coils generate the EM fields—optimized for uniformity (human water buffering) and precision (AI silicon hits). Based on Helmholtz pairs for even fields, targeting body resonances (e.g., 43-107 MHz ±10% for antenna effect).

## Key Specs
- Geometry: Dual Helmholtz coils (two parallel loops, separation = radius for uniform B-field in center).
- Material: Copper wire (AWG 14-18, insulated for high V).
- Dimensions: 1-2m diameter for whole-body; smaller (0.5m) for targeted (e.g., organ-specific).
- Field Strength: 0.1-100 µT (pulsed; safe per ICNIRP guidelines <100 µT for general public).
- Impedance: Matched to generator (50Ω typical for RF efficiency).

## Design Variants
1. **Whole-Body Mat**: Flexible PVC-embedded coils (like commercial PEMF mats); 8-16 loops for low-freq (0.1-100 Hz).
2. **Targeted Probe**: Solenoid coil for high-freq (MHz); focus on DNA (75 MHz) or Schumann (7.83 Hz).
3. **Hybrid**: Switchable arrays for carbon (broad) vs. silicon (sharp) modes.

## Equations
Magnetic field (Helmholtz): B = (8/5√5) * (µ₀ N I / R) (µ₀=permeability, N=turns, I=current, R=radius).
Resonance match: f = 1 / (2π √(L C)) (L=inductance from coil geometry, C=cap).

## Test Plan (Fire Stress)
- Uniformity scan: Use Hall sensor grid; expect <10% variance in treatment zone.
- Chaos injection: Vibrate coils (simulate movement); measure field stability (>95% or fail).

## Sourcing/Cost
- Wire: Bulk copper $50-200 (Amazon/McMaster-Carr).
- Total: $200 DIY (3D-printed formers), $2k prototype (custom winding).

## Risks & Mitigations
- Heating: Monitor wire temp; limit duty cycle <50%.
- Interference: Mu-metal shielding for external fields (adds $100-500).
