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

# Part I :(15 pts)

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

# Part II :(15 pts)

### Part II Deadline: 16/05/2017 03:59

## Part C: Open loop V/f Control

1. Design an **open loop control system** in Simulink for your motor drive. The control system should be capable of controlling the speed with a given reference voltage and frequency data.

2. Starting-up motor:
    - When the motor is stationary under rated load, start the motor with rated voltage and rated frequency. Plot the rotor speed,  current, torque as a function of time.
    - Repeat the previous step with half of the rated voltage and half of the rated frequency. 
    - Compare the two cases and comment. Verify the steady state speed for the above conditions analytically as well.

3. **Analytically** calculate the required voltage and frequency (under constant V/f operation) to run the motor at a 0.1 pu of the rated speed, under rated load. Then verify your analytical calculations with your simulations. Comment for any discrepancies and modify your analytical calculations if required.

# Part III :(30 pts)

### Part III Deadline: 29/05/2017 03:59

## Part D: Closed Loop Control

1. Model the closed loop system you proposed in previous parts, on MATLAB/Simulink.
2. Verify your design by showing a few sample results. Note that, the results should show that your closed loop model works properly. Therefore, include necessary simulation outputs.
3.  Do the following tests using the close loop control:

    * Implement a soft-starting algorithm (the starting current should not exceed twice of the rated current).
    * Show the speed regulation of the drive (Initially set the speed reference to 1000 rpm at rated load. Once the motor reached to steady state, instantaneously remove the load (no-load), and plot the speed and torque generated as a function of time).
    * Measure the speed bandwidth of your drive (i.e. set the speed reference to the rated speed at no load and when machine is operating under steady-state conditions, suddenly set the speed reference to -rated speed (i.e. opposite direction). During the transition plot the relevant figures (i.e. speed, generated torque, current, applied voltage etc.,)
    * Implement flux weakening operating mode (Rotate the motor at 1.5 pu of the rated speed with 0.5 pu of the rated load). Don't forget to keep applied voltage constant at the rated value.

3. Comment on the results of the performance of your closed loop control.


## Part E: Component selection and verification

1. Select suitable **power semiconductor devices** (diodes, IGBTs etc.) for your motor drive system using commercially available product catalogs. **Give your reasonings.**
2. By using your previous simulation results, **verify** your selections can work with all operating conditions (i.e. check the maximum voltage, current, etc).

## Part F: Loss characterization and efficiency calculation

1. Approximately calculate **semiconductor device power losses** using simulation outputs, and device data-sheet parameters. Explain each method, parameter, indicate any external source you have used. It is highly advised to use **application notes** published by the semiconductor device manufacturers.
2. Find the **efficiency** of the motor drive system at the rated conditions. Then calculate the overall efficiency (including the efficiency of the motor). Comment on  the results you found, and discuss how you could achieve a higher efficiency.

**NOTES:**
* There are several ways for loss calculation. Getting accurate results takes too much effort. Therefore, use approximate methods from applications notes.
* The aim of this project is not designing the most optimum or the most efficient motor drive system. Whenever you think the performance of the motor drive is not good, just comment on it and discuss how it can be improved.
* If you find unrealistic values (for example 10% efficiency), go back to your design. It's highly probable that you made a calculation mistake, but if it's really that low, then you need to modify your design.

# Part IV (BONUS) :(20 pts)

### Part IV Deadline: Until the final exam

## Part G: Field oriented control

1. Read about the field oriented control (FOC) for induction motor drives. Give a brief summary (1-2 pages) about the theory of operation.
2. Implement a FOC system to your drive. In this stage, you are free to use readily available models (for example MATLAB has a few nice examples), but don't forget to use your own motor parameters, including the current limits. Define how you calculated reference id and iq values.
3. Start your motor from zero speed to rated speed, and plot the relevant figures. Compare this with starting the motor with direct voltage start and closed-loop V/f control.
4. Implement a bandwidth test as you did with the closed-loop control. Compare and comment the performance of the field oriented control method.

## HINTS:

Comments are the most important section of your project report. Please explain both your models and results as detailed as possible. Please refer to [evaluation sheet](https://github.com/odtu/ee462/blob/master/Project_3/evaluation.md) for details.

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
