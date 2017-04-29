# Project-3: Design of Induction Motor Drive

## Definition

In this project, you will be dealing with:

* Characterization of the motor from the given data
* Designing induction motor drive system for a specific application
  * Drive topology proposition
  * Power stage design
  * Control system design
* Modeling and simulation of the proposed design in MATLAB/Simulink
* Applying open-loop control for different operating modes
* Performance evaluation of the designed drive system
* Applying closed-loop control

As in the previous projects, the model that you will build and your results should be **completely on your own**.

Please see the [motor ratings, design requirements and other parameters assigned to you](https://github.com/odtu/ee462/blob/master/Project_3/motordata.md) .

The available supply is a three-phase AC source and the induction motors are squirrel cage type. The load profile is also assigned to you individually. The induction motor drive system is shown in Fig. 1.

![](./project3.png)

Fig. 1: The induction motor drive system

# Project Content

# Part I :(20 pts)

### Part I Deadline: 09/05/2017 03:59

## Part A: Motor Characterization

1. Using the motor specs and and test data, obtain and plot the **torque-speed characteristics** of the induction motor assigned to you using MATLAB (not Simulink).
2. Determine the starting torque, pull-out torque and the rated torque values, both analytically and label the relevant points in the graph.
3. Plot torque-speed curves at 4 different **Constant Volts/Hertz** combinations on the same graph. Comment on how will affect to have constant E/f compared to constant V/f.

## Part B: Drive proposition

1. Considering the supply, motor and load requirements, propose a **power stage topology** for a four-quadrant speed controlled induction motor drive system. Draw the circuit diagram and explain the components. Give full reasoning.
2. Define the measured parameters (i.e. required sensors) and your control control variables. Explain your proposition.
3. Decide on the components you would like to use, including the switching frequency, DC-link components, power stage switch types, braking resistor (if required) etc. and explain your calculations analytically.
4. Sketch a block diagram showing the closed loop control system and define each part. Note that your diagram may be composed of multiple control stages. Do not copy the control block from the Internet, and explain the subsystems in detail.

**NOTES**
* Although this part has low credit, it is very critical in this project. You will continue with the next parts building on this part.
* Consider all the requirements asked from you, not just a regular drive application.
* Your drive system may be composed of more than one controlled stage. In that case, indicate the asked parameters for all of them.
* Your drive may not be the most optimum one, it is OK. However, your proposition should be reasonable and implementable.

# Part II :(30 pts)

### Part II Deadline: 16/05/2017 03:59

## Part C: Open loop V/f Control

1. Design an **open loop control system** in Simulink for your motor drive. The control system should be capable of controlling the speed with a given reference voltage and frequency data.

2. Starting-up motor:
    - When the motor is stationary under rated load, start the motor with rated voltage and rated frequency. Plot the rotor speed,  current, torque as a function of time.
    - Repeat the previous step with half of the rated voltage and half of the rated frequency. 
    - Compare the two cases and comment. Verify the steady state speed for the above conditions analytically as well.

3. **Analytically** calculate the required voltage and frequency (under constant V/f operation) to run the motor at a rated speed of 0.1 pu under rated load. Then verify your analytical calculations with your simulations. Comment for any discrepancies and modify your analytical calculations if required.


**THE PARTS BELOW ARE STILL IN THE DRAFT VERSION!**

# Part III :(30 pts)

### Part III Deadline: 27/05/2017 03:59

## Part D: Closed Loop Control

1. Model the closed loop system you proposed in previous parts, on MATLAB/Simulink.
2. Verify your design by showing a few sample results. Note that, the results should show that your closed loop model works properly. Therefore, include necessary simulation outputs.
3. Comment on the results.

* Soft-starting the motor (the starting current should not exceed twice of the rated current).

* Speed regulation (from rated load to no load condition)
* Control bandwidth test (from positive to negative speed change)

* Flux weakening range

## Part E: Component selection and verification

1. Select the **power semiconductor devices** (diodes, IGBTs etc.) in your motor drive system using commercially available product catalogs. **Give reasoning.**
2. **Verify** your selections by using the simulation outputs at rated conditions (device voltages, currents etc.).

**NOTE:** You can also utilize your simulation models for component selection where necessary.  

## Part F: Loss characterization and efficiency calculation

1. Calculate **semiconductor device power losses** using simulation outputs, and device datasheet parameters. Explain each method, parameter, approximation and indicate any external source you used. It is highly advised to use **application notes** published by semiconductor device manufacturers.
2. Find the **efficiency** of the motor drive system at the rated conditions. Discuss the results you found.

**NOTES:**
* There are several ways for loss calculation. Getting accurate results takes too much effort. Therefore, use approximate methods from applications notes.
* The aim of this project is not designing the most optimum or the most efficient motor drive system. Whenever you think the performance of the motor drive is not good, comment on it and discuss how it can be improved. Do not try to soap down.
* If you find unrealistic values (for example 10% efficiency), go back to your design. Either you made a critical mistake in the design, or your calculations are not accurate.

# Part IV :(20 pts)

## Part G (BONUS): Operating modes


### Part IV Deadline: Until Final

## Field oriented control

Comments are the most important section of your project report. Please explain both your models and results as detailed as possible. Please refer to [evaluation sheet](https://github.com/odtu/ee462/blob/master/Project_3/evaluation.md) for details.

## HINTS:

* When constructing the models, go **step-by-step**. First built a few components, check if it is working as intended, if it works then add new components. Do not try to implement the whole model at once, expect it to work without any problems.
* Always be aware to use **correct units**.
* Understand the **requirements** before propositions.
* If you have any problems with your models, you can always [open an issue in GitHub](https://guides.github.com/features/issues/) for online feedback, or visit the course assistant and lecturer during their office hours.
*  Do not forget to cite to any external sources you used.

## Submission

You have to commit at least the following files until the deadline:

- MATLAB code(.m file) for characterization
- The Simulink models
- A project report describing your models in detail (Your simulation results should be embedded in your report).
