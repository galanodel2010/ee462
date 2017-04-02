# Project-2: Design of DC motor drive

## Definition

In this project, you will be dealing with:

* Modeling and simulation of four-quadrant DC motor drives with power electronics
* Applying open-loop and closed-loop control
* Circuit design and component selection
* DC motor modes of operation

As in the previous project, the model that you will build and your results should be **completely on your own**.

Please see the [motor ratings, design requirements and other parameters assigned to you](https://github.com/odtu/ee462/blob/master/Project_2/motordata.md) .

The available supply is three-phase grid voltage with 230 Vrms, and 50 Hz ratings. The load profile is also assigned to you individually. The most general motor drive circuit for such a case is shown in Fig. 1.

![](./project2.png)

Fig. 1: The most common 4Q motor drive circuit with 3-phase AC input

# Project Content

# Part I :(70 pts)

### Part I Deadline: 14/04/2017 03:59

## Part A: Preliminary Design

1. Design the filter component values to obtain 1% peak-to-peak ripple voltage at the DC bus (no analytic explanation is necessary, but try to choose realistic values (i.e. in the range of mH and mF)).
2. Decide the switching frequency. Consider the electrical time constant of the motor. The armature current peak-to-peak ripple should not exceed 1%.

NOTE: You may finalize your design with the simulation work in Part B; however, you need to show your theoretical approach in Part A. Applying only "trial and error" method is not accepted.

## Part B: Modeling and Simulation

1. Model the rectifier circuit with the DC link filter. At this stage, just connect a constant resistive load (which represents the power consumption of motor-load combination) and obtain voltage and current waveforms, and show that DC bus voltage ripple is less than 1%. The value of the load resistor, which represents the power output, should be selected according to the rated power output of the motor.

2. Motor-Drive Modeling:
  * Model the 4Q chopper circuit along with the DC motor and the load. Connect a constant ideal DC source to the DC bus (Do not use the rectifier that you designed yet!).
  * Construct a generic PWM subsystem which can generate gate signals for all the transistors separately and can be used for all operation modes (forward motoring, reverse motoring, regenerative braking etc.).
  * Drive the motor with 60% duty cycle PWM in forward motoring mode. Obtain armature voltage, armature current, torque and speed waveforms.

3. Now, combine these two models together and obtain the same characteristics asked previously for both parts. Comment on the differences on the waveforms; i.e., the effect of one side to another.

## Part C: Open Loop Control

In this part, use the combined model (Part B-3). In Simulink, set the initial capacitor voltage close to its steady state value to get rid of the transient effects due to the capacitor charge.

1.  Forward Motoring at Rated Speed:

* Obtain the torque expression of the motor in terms of speed and terminal voltage, at steady state. In addition, obtain the expression of the duty cycle in terms of speed and torque at steady state.
  * Calculate the duty cycle that should be applied to the motor to operate at its rated speed under rated load torque, in forward motoring mode (i.e. train is accelerating, elevator going up).
  * Apply the proper gate signals to the chopper according to your calculation and obtain armature voltage, current, torque and speed waveforms. The initial motor speed should be zero.
  * Comment on the results.

2.  Rated Speed to Half Speed Step Response:

* Calculate the duty cycle that should be applied to the motor to operate at half of its rated speed under rated load torque, in forward motoring mode.
  * Apply a step change to the duty cycle applied to the motor drive from the value in (1) to (2). Obtain the armature voltage, armature current, torque and speed waveforms adter the speed reference has been halved.
  * Comment on the results and the operating modes. Comment on the limitations on this topology if the regenerative braking applied for a long time.

---

# Part II (30 pts)

### Part II Deadline:
25/04/2017 03:59


## Part D: Dynamic Braking

3. Design of the Dynamic Brake System: In the previous part you should have observed the DC-link voltage increases dangerously. To prevent that a braking resistor should be used.

* What will happen when the drive is kept in the braking state for a long time without the braking resistor? Prove your statement with simulation outputs (i.e. DC-link capacitor voltage, braking torque vs. time).

* Choose the ratings of the dynamic braking resistor (i.e. resistance, current rating, voltage rating). 

* Implement a dynamic braking circuit such that the DC-link voltage does not exceeds 750Vdc.


## Part E: Closed Loop Control:

1. Propose and implement a PI (or PID) type **current controller** for the DC motor drive for start-up. The aim is to accelerate the motor from standstill to its rated speed with a current that does not exceed 150% of its rated current (hence 150% of its rated torque) at forward motoring mode. Constant load torque (rated) should be applied to the motor. Obtain armature voltage, current, speed and the variation of applied duty cycle during start-up.

2. Propose and implement a hysteresis (on-off) type current controller for the DC motor drive for start-up. The same requirements and specifications are valid as in (1). Obtain armature voltage, current, torque and speed waveforms.

3. Compare the two methods and comment. What are the advantages and disadvantages of each method.

---
# Part III (25 pts Bonus)
Deadline: 25/04/2017 03:59

## Part F: Speed Controller

1. Now, add a speed controller to your model, which generates the torque (or current) reference for the current controller. Notice that, this reference was applied by hand in the previous part. Now, the two control loops are combined together. This method is called double loop control. Also note that, speed reference will be set by the user, this time.

2. Accelerate your system from standstill to rated speed and show that both your speed controller and current controller works as expected. Comment on the performance of your controller.

3. Then, implement a controller such that, your system can accelerate and decelerate according to maximum limits defined in your motor specs. You can also implement the jerk limits in your controller.


### Part G: Component Selection

1. What may be most suitable power semiconductor type for this application? Give reasoning (i.e. which type of MOSFET or IGBT, etc)

2. Select a commercially available transistor (with anti-parallel diodes) and explain your reasoning. Use simulation outputs to prove your statement. (You can start your search from [Semikron](https://www.semikron.com/products/product-classes/igbt-modules.html), [ABB](http://new.abb.com/semiconductors) catalogues)

3. Select rectifier diodes. (You can start your search from [Semikron](https://www.semikron.com/products/product-classes/igbt-modules.html), [ABB](http://new.abb.com/semiconductors) catalogues)

Comments are the most important section of your project report. Please explain both your models and results as detailed as possible. This part does not need to be a separate part, but the comments can be included after each analysis part. Please refer to [evaluation sheet](https://github.com/odtu/ee462/blob/master/Project_1/evaluation.md) for details.


## HINTS:

* When constructing the models, go **step-by-step**. First built a few components, check if it is working as intended, if it works then add new components. Do not try to implement the whole model at once, expect it to work without any problems.
* Always be aware to use **correct units**.
* Understand the **analytical model** before constructing the models.
* If you have any problems with your models, you can always [open an issue in GitHub](https://guides.github.com/features/issues/) for online feedback, or visit the course assistant and lecturer during their office hours.
*  Do not forget to cite to any external sources you used.

## Submission

You have to commit at least the following files until the deadline:

- The Simulink models (either as three separate files or a combined model)
- A project report describing your models in detail (Your simulation results should be embedded in your report).
