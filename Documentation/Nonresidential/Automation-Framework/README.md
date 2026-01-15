# Automation Framework: Nonresidential Prototypes

This directory contains supporting database files used by the **automation framework** to develop, manage, and simulate the **California Nonresidential Prototype** building models.

The automation workflow references the following CSV inputs:

### `ENVELOPE.csv`
Defines the building envelope performance by building type, climate zone, and code era. It uses Prototype, CZ, and Vintage to select the correct envelope values for each location. The file specifies window glazing properties, including overall U-factor, solar heat gain coefficient (SHGC), and visible transmittance, and insulation material properties for walls and roofs, such as insulation thickness and target assembly U-factors. These inputs are used by the workflow to generate consistent EnergyPlus envelope materials and to calibrate or validate envelope performance across different climates and vintages.


### `WHOLE_BLDG.csv`
Defines building-level loads and systems that are not tied to individual zones but apply to the entire building. It uses Prototype and Vintage to select the correct values by building type and code era, then specifies whole-building objects such as exterior lighting, exterior fuel/electric equipment (for example elevators), and central water heaters. For each of these, it provides names, schedules, capacities or power levels, control options, and reporting tags. The workflow reads this file to automatically create consistent EnergyPlus whole-building objects, keeping site loads and central systems separate from zone-level inputs.

### `ZONE.csv`
Defines what each building zone is and how it behaves in the energy model. It identifies which building type and code era the zone belongs to, then describes the zone’s size and whether it counts toward total floor area. It also specifies all major zone inputs: people, lighting, plug loads, gas loads, infiltration, ventilation, hot water use, and thermostat setpoints, using simple values and schedules. The file is used by the workflow to automatically create consistent EnergyPlus zone objects and internal loads without manually editing the model.