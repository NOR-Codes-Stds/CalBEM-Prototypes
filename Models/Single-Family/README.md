# Single-Family
There are four types of IDF models available in the Single-Family folder, including:
  
  - `Model A`: 1-Story Single-Family home with a conditioned floor area of 1250 SF.
  
  - `Model B`: 1-Story Single-Family home with a conditioned floor area of 1750 SF.
  
  - `Model C`: 2-Story Single-Family home with a conditioned floor area of 2250 SF.
  
  - `Model D`: 2-Story Single-Family home with a conditioned floor area of 2750 SF.

  
## Revision 2 — Single‑Family Prototype Models

 - Scope: This release incorporates targeted corrections and calibration updates for the second revision of the single‑family residential EnergyPlus prototype set.

    - Detailed Single-Family Change Log
        - Model A: Building Envelope: Window Overhang Geometry - Re‑defined overhang vertex coordinates to eliminate shading‑object misalignment.
        - Model C: Spatial Layout: Second‑Floor Inter‑Zone Spacing - Corrected surface‑adjacency definitions to resolve conditioned/unconditioned‑zone gaps.
        - All models: Infiltration: ACH Rates (2006 – 2022 & New‑Construction Vintages) - Adjusted infiltration rates to meet minimum ventilation requirements (per ASHRAE 62.2‑2022 and CA Title 24).
        - All models: Domestic Hot Water: DHW End‑Use Calibration - Re‑parameterised storage‑tank settings and distribution piping to align annual hot‑water energy use with Residential Appliance Saturation Study (RASS) Unit Energy Consumption (UEC) targets.
