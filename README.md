
# Crude Oil Pipeline System Design

## Project Description

This project involves the design of a pipeline system in a petroleum refinery to pump crude oil from the storage area to the atmospheric distillation unit. [cite: 2] The design process includes determining the optimum pipe diameter, selecting an appropriate pump, and calculating the total yearly cost of the system. [cite: 5, 6]

## Objectives

* Determine the optimum pipe diameter for the crude oil pipeline system. [cite: 5]
* Select a suitable pump for the pipeline system. [cite: 5]
* Calculate the yearly total cost of the pipeline system. [cite: 6]

## Input Data

The following input data is used for the design calculations.

### Table 1: Distribution of Parameters

| Person                       | Volumetric Flow Rate (m³/h)  | Total Length of Piping (m)   | API Gravity of Crude Oil at 60°F | Viscosity of Oil in SUS at 60°F|
| :-------------------------   | :--------------------------: | :--------------------------: | :------------------------------: | :-----------------------------:|
| Alper Medet                  |              15              |             200              |                20                |               200              |
| Bahar Aylin Çakır            |              15              |             250              |                15                |               220              |
| Cemre Nur Deveci             |              15              |             350              |                25                |               180              |
| Abdirrahman Osman Daror      |              20              |             400              |                30                |               240              |
| Fatma Nur Çapar              |              20              |             200              |                25                |               220              |
| Nil Teber                    |              20              |             250              |                20                |               180              |
| Ghene Allaia                 |              25              |             350              |                30                |               200              |
| Tamim Abdo Ahmed Ali Aljabri |              25              |             400              |                30                |               180              | [cite: 8]

### Table 2: Price List for Sch. 40 Steel Pipes

| Nominal Diameter, in.  | Price, \$/m |
| :--------------------: | :---------: |
|          1/2           |     1.5     |
|          3/4           |     1.9     |
|            1           |     2.7     |
|          1 1/4         |     3.5     |
|          1 1/2         |     4.0     |
|            2           |     5.6     |
|          2 1/2         |     7.3     |
|            3           |     9.5     |
|            4           |    14.0     |
|            5           |    20.1     |
|            6           |    23.3     |
|            8           |    34.0     |
|           10           |    46.9     |
|           12           |    60.2     | [cite: 10]

## Piping System Details

* Entrance pressure: Atmospheric [cite: 3]
* Exit gauge pressure: Equivalent to a head of 20m of crude oil [cite: 3]
* Piping system components:
    * 3 gate valves fully open [cite: 4]
    * 2 gate valves half open [cite: 4]
    * 2 globe valves fully open [cite: 4]
    * 10 elbows [cite: 4]
    * 5 U-turns [cite: 4]
    * 3 tees with flow through run [cite: 4]
    * 2 tees with flow through branch [cite: 4]
* Piping system operation: 350 days per year [cite: 5]
* Service life: 10 years [cite: 5]
* Electricity cost: 0.075 \$/kW-hr [cite: 11]
* Piping installation cost: 25% of the purchase cost [cite: 11]

## Work Packages

### WP1: Project Setup and Fluid Properties

* **Description:** This WP focuses on setting up the project repository, defining the scope, and determining the fluid properties of the crude oil.
* **Tasks:**
    1.  Create a GitHub repository and initialize the project.
    2.  Define project scope and objectives.
    3.  Obtain crude oil properties (API gravity, viscosity) from Table 1.
    4.  Calculate the density of the crude oil.
* **Deliverables:**
    1.  GitHub repository setup.
    2.  Project scope document.
    3.  Document outlining the fluid properties of the crude oil.

### WP2: Piping System Design and Analysis

* **Description:** This WP involves designing the piping system, including pipe diameter selection, and analyzing the fluid flow.
* **Tasks:**
    1.  Determine the equivalent length of the piping system, considering valves, fittings, and pipe length.
    2.  Select appropriate pipe diameters (using Table 2) and calculate the flow velocity for each diameter.
    3.  Calculate the Reynolds number and determine the flow regime (laminar or turbulent).
    4.  Calculate the friction factor and head loss for each pipe diameter.
    5.  Determine the total head required by the pump.
    6.  Evaluate different pipe diameters to find the optimum diameter based on cost and performance.
* **Deliverables:**
    1.  Piping system layout diagram.
    2.  Calculations for flow velocity, Reynolds number, friction factor, and head loss.
    3.  Optimum pipe diameter selection report with justification.

### WP3: Pump Selection and Analysis

* **Description:** This WP focuses on selecting a suitable pump for the piping system and analyzing its performance.
* **Tasks:**
    1.  Determine the required pump head and flow rate.
    2.  Select a pump type and model that meets the system requirements.
    3.  Obtain pump performance curves.
    4.  Calculate the pump's operating power.
* **Deliverables:**
    1.  Pump selection report with specifications.
    2.  Pump performance analysis.

### WP4: Cost Analysis

* **Description:** This WP involves calculating the capital and operating costs of the piping system.
* **Tasks:**
    1.  Calculate the cost of pipes based on the selected diameter and total length (using Table 2).
    2.  Calculate the piping installation cost (25% of pipe purchase cost). [cite: 11]
    3.  Estimate the pump purchase cost.
    4.  Calculate the annual operating cost, considering electricity consumption (0.075 \$/kW-hr) and operating hours (350 days/year). [cite: 11]
    5.  Calculate the total yearly cost of the system.
    6.  Perform a 10-year cost analysis.
* **Deliverables:**
    1.  Capital cost estimation report.
    2.  Operating cost estimation report.
    3.  Total yearly cost calculation.
    4.  10-year cost analysis report.

### WP5: Documentation and Reporting

* **Description:** This WP focuses on documenting the entire project and preparing the final report.
* **Tasks:**
    1.  Compile all the results and analyses into a final report.
    2.  Prepare an abstract, introduction, and conclusion.
    3.  Create a table of contents.
    4.  Document assumptions and sample calculations.
    5.  Include all relevant data, calculations, graphs, and program outputs in the appendix.
* **Deliverables:**
    1.  Final project report in PDF format, adhering to the specified format.

## Report Format

The final report should include the following sections:

1.  Title Page
2.  Table of Contents
3.  Abstract
4.  Introduction
5.  Assumptions and Sample Calculations
6.  Results
7.  Discussions
8.  References
9.  Appendix (Computer program, outputs of the program, graphs, tables used, and other additional information used in the preparation of the report.) [cite: 11]
