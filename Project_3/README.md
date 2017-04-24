# Project-3: Design of induction motor drive

## Definition

In this project, you will be dealing with:

* Characterisation of the motor from the given data
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

### Part I Deadline: 05/05/2017 03:59

## Part A: Motor characterisation

1. Using the motor rated values and test data, obtain the torque-speed curve of the induction motor assigned to you.
2. Determine starting torque, pull-out torque and rated torque values.
3. Plot torque-speed curves at 4 different V/f combinations on the same graph.

## Part B: Drive proposition

1. Considering the supply, motor and load requirements, propose a power stage topology for you motor drive system. Draw the circuit diagram and explain the components. Give full reasoning !
2. Propose the measured paramaters (sensing) and control variable(s). Explain your proposition.

**NOTES**
* Although this part has low credit, it is very critical in this project. You will continue with the next parts building on this one.
* Consider all the requirements asked from you, not just a regular drive application.
* Your drive system may be composed of more than one controlled stage. In that case, indicate the asked parameters for all of them.
* Your drive may not be the most optimum one, it is OK. But, your proposition should be reasonable.

# Part II :(30 pts)

### Part II Deadline: 12/05/2017 03:59

## Part C: Modeling and open loop control


# Part III :(30 pts)

### Part III Deadline: 19/05/2017 03:59

## Part D: Component selection and verification


## Part E: Loss characterisation and efficiency calculation

## Part F: Performance evaluation


# Part IV :(20 pts)

### Part IV Deadline: 26/05/2017 03:59

## Part G: Operating modes

## Part H: Closed loop control


# Part V :(20 pts-bonus)

### Part V Deadline: 02/06/2017 03:59

## Field oriented control

# Part VI :(20 pts-bonus)

### Part VI Deadline: 09/06/2017 03:59

## PWM rectifier


Comments are the most important section of your project report. Please explain both your models and results as detailed as possible. Please refer to [evaluation sheet](https://github.com/odtu/ee462/blob/master/Project_3/evaluation.md) for details.

## HINTS:

* When constructing the models, go **step-by-step**. First built a few components, check if it is working as intended, if it works then add new components. Do not try to implement the whole model at once, expect it to work without any problems.
* Always be aware to use **correct units**.
* Understand the **requirements** before propositions.
* If you have any problems with your models, you can always [open an issue in GitHub](https://guides.github.com/features/issues/) for online feedback, or visit the course assistant and lecturer during their office hours.
*  Do not forget to cite to any external sources you used.

## Submission

You have to commit at least the following files until the deadline:

- MATLAB code for characterisation
- The Simulink models
- A project report describing your models in detail (Your simulation results should be embedded in your report).
