# CalBEM-Prototypes

## California Prototypes Development Project
The objective of the California Prototypes Development project, funded by Southern California Edison’s (SCE) Codes and Standards Program, is to develop a set of prototype building models representing California’s residential and nonresidential building stock that can be used by policymaking agencies and other stakeholders. Prototypes developed under this project attempt to capture features of California’s building stock using the latest data sources. The models and model inputs development were developed with input from a technical advisory group (TAG) and underwent review from several parties during the development process. The models and the underlying model inputs and assumptions have been documented and can be accessed from this page.

## Residential Prototypes Status

Single family and low-rise multifamily models are available for testing and review. Specifications for these models and the model input development and validation documentation is also available. High-rise multifamily prototypes are under development.

## Nonresidential Prototypes Status

Nonresidential prototype development is currently underway. The initial steps of evaluating the building stock, vintage binning, and defining of prototypes have been completed. Currently, office prototype inputs are being developed. The Small Office and Medium Office prototype models and specifications are expected to be released for review and testing by Spring 2025.

## Downloads

- [Models](https://github.com/NOR-Codes-Stds/CalBEM-Prototypes/tree/main/Models)
- [Specifications](https://github.com/NOR-Codes-Stds/CalBEM-Prototypes/tree/main/Specifications)
- [Documentation](https://github.com/NOR-Codes-Stds/CalBEM-Prototypes/tree/main/Documentation)

## Project Background

Currently, multiple sets of prototype models are being used by policymaking agencies to perform analyses in California. Government agencies, private entities, consultants, and other market actors use models that are accessible to them, resulting in a lack of uniformity in predicted outcomes and confusion about which models are appropriate for use. The CalBEM Prototypes project aims to change this current market state.

The Prototypes Project scope includes the development of prototype models for single-family, multifamily, and nonresidential building sectors. As part of this project, a Technical Advisory Group (TAG) was convened comprising the CEC, CPUC, SCE, NORESCO, Energy Solutions, and other interested parties, including DOE national laboratories and national experts. This TAG has guided the development of the prototype models. NORESCO leads the technical development of the prototype models and Energy Solutions has managed the project on behalf of SCE. The TAG meets on a bi-monthly basis and has been meeting since the beginning of 2021 to develop the project framework and guide model development.

For each of the three building sectors (single-family, multifamily, and nonresidential), the development of prototype models was divided into four major tasks:

1. Building stock assessment: Characteristics of the building stock were reviewed and evaluated so that representative models of those buildings can be developed. Based on the stock assessment, a mix of prototype models was selected to represent key characteristics of buildings within the California stock, such as building floor area, number of dwelling units, number of stories, etc.
1. Model inputs development: Once prototype models that will represent the stock were identified, each prototype was characterized further in terms of  various building systems, such as the envelope, lighting, HVAC, water heating, plug and process loads, and other energy systems. The inputs needed to define these systems were developed and associated calculations and assumptions were documented. A specification for each prototype has been developed with the intent of maintaining engine neutrality, i.e., using the model specification, the prototype model can be developed using any simulation engine. 
1. Model construction: Using the inputs developed in the previous step, models were constructed in DOE’s EnergyPlusTM simulation engine. The intent was to host these EnergyPlusTM models as well as the underlying input assumptions in a publicly accessible workspace, so that all entities can share and use the same prototype models. Feedback received on the models will be incorporated into future versions.
1. Validation: Prototype models were validated at the end-use level using stock energy consumption data from the 2019 Residential Appliance Saturation Survey (RASS) for single-family and multifamily buildings. The 2022 Commercial End-Use Survey (CEUS) will be used, for validating nonresidential buildings. 

Model input documentation and the open nature of dialogue and collaboration between  stakeholders via the Prototypes TAG are key features of this project. The intent is to rigorously document the assumptions, host the models and documentation on a public platform, and provide a forum for continuous improvement, maintenance, and development.

## Revision 2 — Single‑Family Prototype Models

 - Scope: This release incorporates targeted corrections and calibration updates for the second revision of the single‑family residential EnergyPlus prototype set.

    - Detailed Change Log
        - Model A: Building Envelope: Window Overhang Geometry - Re‑defined overhang vertex coordinates to eliminate shading‑object misalignment.
        - Model C: Spatial Layout: Second‑Floor Inter‑Zone Spacing - Corrected surface‑adjacency definitions to resolve conditioned/unconditioned‑zone gaps.
        - All models: Infiltration: ACH Rates (2006 – 2022 & New‑Construction Vintages) - Adjusted infiltration rates to meet minimum ventilation requirements (per ASHRAE 62.2‑2022 and CA Title 24).
        - All models: Domestic Hot Water: DHW End‑Use Calibration - Re‑parameterised storage‑tank settings and distribution piping to align annual hot‑water energy use with Residential Appliance Saturation Study (RASS) Unit Energy Consumption (UEC) targets.