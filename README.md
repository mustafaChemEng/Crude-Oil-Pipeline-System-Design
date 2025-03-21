# Fluid Mechanics - Pipeline Design for Petroleum Refinery

This repository contains a C++ program designed to determine the optimum pipe diameter and pump type for a pipeline system in a petroleum refinery. The system pumps crude oil from a storage area to an atmospheric distillation unit.

## Project Description

The project involves designing a pipeline system with the following specifications:

* **Objective:** Determine the optimal pipe diameter and pump type for a crude oil pipeline.
* **Application:** Petroleum refinery, pumping crude oil from storage to an atmospheric distillation unit.
* **Constraints:**
    * Entrance pressure is atmospheric.
    * Exit gauge pressure corresponds to a 20m head of crude oil.
    * The piping system includes:
        * 3 gate valves (fully open)
        * 2 gate valves (half open)
        * 2 globe valves (fully open)
        * 10 elbows
        * 5 U-turns
        * 3 tees (flow through run)
        * 2 tees (flow through branch)
* **Optimization Criteria:** Cost (including pipe, installation, pump, and electricity).
* **Operational Parameters:**
    * Operation: 350 days/year
    * Service life: 10 years

## Input Data

The program utilizes the following input data:

* **Table 1: Distribution of Parameters for each group** [cite: 7, 8]

    | Group | Volumetric Flow Rate (m³/h) | Total Length of Piping (m) | API Gravity of Crude Oil at 60°F  | Viscosity of Oil in SUS at 60°F |
    | ----- | --------------------------- | -------------------------- | --------------------------------- | -----------------------------   |
    | 1     | 15                          | 200                        | 20                                | 200                             |
    | 2     | 15                          | 250                        | 15                                | 220                             |
    | 3     | 15                          | 350                        | 25                                | 180                             |
    | 4     | 20                          | 400                        | 30                                | 240                             |
    | 5     | 20                          | 200                        | 25                                | 220                             |
* **Table 2: Price List for the Sch. 40 Steel Pipes** [cite: 9, 10]

    | Nominal Diameter, in. | Price, \$/m |
    | --------------------- | ----------- |
    | 1/2                   | 1.5         |
    | 3/4                   | 1.9         |
    | 1                     | 2.7         |
    | 1 1/4                 | 3.5         |
    | 1 1/2                 | 4.0         |
    | 2                     | 5.6         |
    | 2 1/2                 | 7.3         |
    | 3                     | 9.5         |
    | 4                     | 14.0        |
    | 5                     | 20.1        |
    | 6                     | 23.3        |
    | 8                     | 34.0        |
    | 10                    | 46.9        |
    | 12                    | 60.2        |

* **Other Costs:**
    * Piping installment cost: 25% of the purchase cost [cite: 11]
    * Cost of electricity: 0.075 \$/kW-hr [cite: 11]

## Program Details

###   Language

    * C++

###   Functionality

    * Calculates fluid properties (density, viscosity).
    * Calculates flow parameters (velocity, Reynolds number, friction factor, head loss).
    * Calculates pump parameters (pump head, pump power).
    * Estimates costs (pipe, installation, pump, electricity).
    * Determines the optimum pipe diameter based on cost minimization.
    * Calculates the yearly total cost of the system.

###   Code Structure

    * The code is organized into functions for each calculation (e.g., `calculateDensity`, `calculateFlowVelocity`, `calculateTotalCost`).
    * Data structures (`PipeData`, `CrudeOilData`, `PipeResult`) are used to store and organize data.

## How to Use

1.  **Clone the repository:**
    ```bash
    git clone <repository_url>
    ```
2.  **Compile the code:**
    ```bash
    g++ <your_code_file.cpp> -o <output_executable>
    ```
3.  **Run the executable:**
    ```bash
    ./<output_executable>
    ```

## Output

The program outputs:

* The optimum pipe diameter.
* The yearly total cost of the system.
* Detailed results for each pipe diameter considered, including flow parameters and cost components.

## Assumptions

* The code uses simplified approximations for some calculations (e.g., turbulent flow friction factor, pump cost).
* Specific K-values for fittings are assumed and may need to be adjusted for a real-world application.
* Pump selection and costing are simplified. A real-world application would require consulting pump vendor data.

## Disclaimer

This program provides a simplified model for pipeline design. It should not be used for actual engineering design without further validation and consideration of all relevant factors.
