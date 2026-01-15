# Automation Framework: Nonresidential Prototypes

This directory contains supporting database files used by the **automation framework** to develop, manage, and simulate the **California Nonresidential Prototype** building models.

The automation workflow references the following CSV inputs:

### `ENVELOPE.csv`
Database of **building envelope constructions** used by the nonresidential prototypes (e.g., walls, roofs, floors, fenestration assemblies).  
This file defines the construction types and mappings used when generating prototype envelope inputs.


### `WHOLE_BLDG.csv`
Database of **whole-building EnergyPlus objects** that apply at the building level (not zone-specific), including:
- `Exterior:Lights`
- `WaterHeater:Mixed`
- `Exterior:FuelEquipment` (e.g., elevator-related loads)

### `ZONE.csv`
Database of **zone definitions** used by the nonresidential prototypes.  
This file establishes the zones applicable to each prototype and supports automation tasks.