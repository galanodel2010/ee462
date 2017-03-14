# Project-1: Modeling a DC-motor drive system

## Definition

In this project, you will be dealing with:

* Modeling a DC motor drive system using various techniques
* Building a simple DC motor drive on your own
* Analysis of the electrical and mechanical characteristics and comment

You may investigate some ready-prepared models you find on the internet, however the model that you will build and your results should be completely on your OWN.

Please see the motor ratings and other parameters assigned to you. The motor drive system that you will model is shown in Fig. 1.

![](./project1.png)

Fig. 1: The DC-motor drive system

## Deadline:
27/03/2017 23:59

## HINTS:

* When constructing the models, go **step-by-step**. Do not try to implement the whole model at once, expect it to work without any problems.
* Always be aware to use correct **units**.
* Understand the **analytical model** before constructing the models
* If you have any problems in a step, you can always [open an issue in GitHub](https://guides.github.com/features/issues/) for online feedback, or visit the course assistant in the office hours.

## Submission

You have to submit at least the following two files:

- The Simulink models
- A report describing your models in detail, with the parts explained below:

Your report should include:
-
-

## Project Content

#### Part A: Modeling

1.	Obtain the **analytical model** of this system (you do not need to show, but you will use it in the second part). The content of your model will include, but not limited to, terminal equation, back emf equation, torque balance equation etc.

2.	Construct a model of this system using **simple Simulink blocks**, such as constant, product, sum, gain, integrator etc. In this part, you are not allowed to use any electrical equipment and Simscape or SimPowerSystem toolbox.

3.	Construct a model of this system using only **sources** (dependent or independent), and **passive elements** (resistors, inductors and capacitors). In this part, you will use SimPowerSystem toolbox, but not use the DC motor block.

4.	Construct a model of this system using the **DC motor** block and SimPowerSystem toolbox.

#### Part B: Analysis

You will apply these analyses to all three models that you have constructed.

1. Apply rated voltages to both field and armature. Obtain the following variations against time. Make sure that the system reaches its steady state. Plots in each part should be on the same axis.
   * Motor speed and torque
   *	Armature voltage and current
   *	Motor torque and load torque
   *	Motor speed and load speed
2.	Apply a stepped armature voltage until its rated value such that the armature current never exceeds 150% of its rated value.
   *	Motor speed and torque
   *	Armature voltage and current
	 *  Motor torque and load torque
   *  Motor speed and load speed
3.	Decrease the field voltage to its 50% when the systems operates at its steady state with its rated values initially.
   *	Motor speed and torque
   *	Armature voltage and current
   *	Motor torque and load torque
   *	Motor speed and load speed
4.	Load torque variations
   *	Motor speed and torque
   *	Armature voltage and current
   *	Motor torque and load torque
   *	Motor speed and load speed


#### Part C: Comments
1.


<!--- Hazır motor dataları
http://w3app.siemens.com/mcms/infocenter/dokumentencenter/ld/Documentsu20Catalogs/dc-motor/da12-2008-en.pdf
http://ecatalog.weg.net/files/wegnet/WEG-specification-of-electric-motors-50039409-manual-english.pdf
http://www.maxonmotor.com/maxon/view/category/motor?target=filter&filterCategory=DC-max
http://www.kollmorgen.com/en-us/products/motors/brush-dc/permanent-magnet-dc-pmdc/
http://www.moog.com/literature/MCG/moc23series.pdf
-->
