# Grid search optimization simulation data 

This repository contains the grid search optimization simulation data output for the paper: **Design and Experimental Verification of a Jumping Legged Robot for
Martian Lava Tube Exploration.**


Simulations were performed in Matlab Simscape multibody with a simplified physical model containing the body with two 5-bar legs, each leg consisting of hips, calves, and a paw. Height is measured from the center of the simulated robot body  at the point where the rotational joints representing the actuators in the 5-bar leg are located. The grid search parameters are listed in the table below.


## Result of the simulations

| Simulation parameter  | Parameter range |
| ------------- | ------------- |
| Hip length  | 0.1 - 0.3 m |
| Calf length  | 0.15 - 0.45 m |
| Spring stiffness  | 600 - 1000 N/m |



The Figure below is a 4D representation of the simulation results, illustrating the jump height for both the symmetric/diamond 5-bar design and the parallel 5-bar design based on varying hip length, calf length, and spring stiffness. All other parameters, such as weight, squat angle, motor power output, and gravity, were held constant for both simulations.

| Simulation parameter  | Parameter value |
| ------------- | ------------- |
| Motor toque  | 21.6 Nm |
| squat angle  | 120 deg |


![Diamond_vs_parallel](https://github.com/ntnu-arl/jumping-robots/assets/47317437/3fb1a3e2-c87f-4e2d-a7d4-7f82be486bf4)


## Data from simulations

Files named 'parallel_sim_data.csv' and 'symetric_sim_data.csv' are the simulation results for the  grid search simulations for parallel and symmetric/diamond  5-bar configurations, respectively.


CSV files contain the following data in each column:


| Column number  | Column content |
| ------------- | ------------- |
| 1  | Simulation counter |
| 2  | Outer loop iteration number |
| 3  | Middle loop iteration number  |
| 4  | Inner loop iteration number  |
| 5  | Body max position |
| 6  | Body min position  |
| 7  | Body nominal position  |
| 8  | Zeros  |
| 9  | Paw max position  |
| 10  | Paw min position  |
| 12  | Paw nominal position |
| 13  | Hip length  |
| 14  | Hip length  |
| 15  | Calf length  |
| 16  | Calf length |
| 17  | Spring coefficient  |
| 18  | Body max position minus body nominal position  |
| 19  | Calf length divided by hip length  |
