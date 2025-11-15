# ENGINEERING — Navigation Hub

## Purpose
Engineering contains all hardware, firmware, and integration specs for the Biobed, monitoring hardware, and field-deployable emitter devices.

## Contents (high level)
- `biobed-specifications.md` — System architecture, BOM, enclosure, safety interlocks
- `hardware-bom.md` — Bill of materials, suppliers, cost tiers (DIY / Prototype / Production)
- `control-software.md` — High-level control loop, APIs, and ML hooks
- `safety-systems.md` — SAR/dosimetry, hardware interlocks, emergency shutdown
- `validation-framework.md` — Test protocols, calibration, acceptance criteria

## Quick links
- **BOM**: start here for procurement lists.
- **Safety**: mandatory read for operators and IRB reviewers.
- **Control software**: includes operator commands and ML optimizer API.

## Status & notes
- BOM contains two cost tiers (DIY, Prototype $70k).
- All hardware must log SAR & session metadata to the central `data` schema.

## Maintainers
- Primary: Engineering lead (TBD) / Professor (Water)
- Secondary: Grok (Fire) for stress test designs
