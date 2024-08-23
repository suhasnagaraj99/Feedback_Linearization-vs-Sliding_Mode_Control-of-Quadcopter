
# Feedback Linearization vs. Adaptive Sliding Mode Control for a Quadrotor Helicopter

## Aim

To study and compare two different approaches for controlling a highly coupled nonlinear system (quadrotor). The aim of this project is to study the research paper and recreate the results.

## Journal Paper

Daewon Lee, H. Jin Kim, and Shankar Sastry, “Feedback Linearization vs. Adaptive Sliding Mode Control for a Quadrotor Helicopter”, International Journal of Control, Automation, and Systems (2009) 7(3):419-428.

## Software Requirements

To run these simulations, you will need:
- MATLAB Simulink with all relevant Toolboxes and support packages.

## Contents

The `Simulations` folder contains the following files:

1. **Feedback_Linearization.slx**: Simulink file for controlling the quadcopter model using a Feedback Linearization Controller.
   
2. **ASMC_without_Sensor_Noise.slx**: Simulink file for controlling the quadcopter model using an Adaptive Sliding Mode Controller (ASMC) without sensor noise.

3. **ASMC_with_Sensor_Noise.slx**: Simulink file for controlling the quadcopter model using an Adaptive Sliding Mode Controller (ASMC) with sensor noise.

4. **plot_3d.m**: MATLAB script to plot the 3D trajectory of the quadcopter.

## How to Run the Simulations

### Running Feedback_Linearization.slx

1. Open `Feedback_Linearization.slx` in Simulink.
2. Go to the **Modeling** tab and select **Model Settings**.
3. Set the following parameters in the settings:
   - **Solver type**: Fixed-Step
   - **Solver**: ode1be
   - **Fixed-Step size**: 0.1
   - **Number of Newton's Iterations**: (Set appropriately)
4. Set the stop time to **30 seconds**.
5. Run the model.
6. Open the individual Scopes to visualize the outputs.
7. Run `plot_3d.m` in MATLAB to visualize the quadcopter's trajectory in 3D.

### Running ASMC_with_Sensor_Noise.slx

1. Open `ASMC_with_Sensor_Noise.slx` in Simulink.
2. Go to the **Modeling** tab and select **Model Settings**.
3. Set the following parameters in the settings:
   - **Solver type**: Fixed-Step
   - **Solver**: auto
   - **Fixed-Step size**: 0.1
4. Set the stop time to **30 seconds**.
5. Run the model.
6. Open the individual Scopes to visualize the outputs.
7. Run `plot_3d.m` in MATLAB to visualize the quadcopter's trajectory in 3D.

### Running ASMC_without_Sensor_Noise.slx

1. Open `ASMC_without_Sensor_Noise.slx` in Simulink.
2. Go to the **Modeling** tab and select **Model Settings**.
3. Set the following parameters in the settings:
   - **Solver type**: Fixed-Step
   - **Solver**: auto
   - **Fixed-Step size**: 0.1
4. Set the stop time to **30 seconds**.
5. Run the model.
6. Open the individual Scopes to visualize the outputs.
7. Run `plot_3d.m` in MATLAB to visualize the quadcopter's trajectory in 3D.

## Credits

This project is based on the research paper by Daewon Lee, H. Jin Kim, and Shankar Sastry titled, “Feedback Linearization vs. Adaptive Sliding Mode Control for a Quadrotor Helicopter” published in the *International Journal of Control, Automation, and Systems* (2009) 7(3):419-428. The simulations and models are developed to replicate and analyze the results discussed in this paper.

## Notes

- Ensure that all required toolboxes and support packages for Simulink are installed and configured properly.
- Follow the steps carefully for each simulation to achieve accurate results.
