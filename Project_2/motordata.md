## Project 2 - Data-Sheets

## How to choose the motor-load combination?

The motor parameters will be assigned randomly, based on the last digit of your student number. For example if your student number is 1244839, then take the modulus 5 of the last digit:

mod-5 (9) = 4

Then you need to use the parameters of the Motor#4 for your project.

## Motor Data-Sheet

In this project, there will be 5 different applications where motor ratings, mechanical properties and load conditions will be different.

#### Application-0: 100 kW light rail vehicle (LRV) traction system.
#### Application-1: 3 MW locomotive traction system.
#### Application-2: 50 kW elevator system.
#### Application-3: 30 kW crane hoist system.
#### Application-4: 1 kW ... motor


Please refer to the data according to the number you are assigned to.

| DC motor| Motor#0| Motor#1| Motor#2| Motor#3| Motor#4|
| :-----: |:-----:| :----:|:-----:| :----:|:-----:|
| Rated armature voltage (V) | 70 | 48 | 24 | 90 | 12 |
| Rated output power (W)| 250 | 192 | 121 | 359 | 26 |
| Rated speed (rpm)  | 2490 | 3226 | 2700 | 1517 | 4700 |
| Armature resistance (Ω)    | 1.41 | 0.7 | 0.43 | 1.45 | 0.6 |
| Armature inductance (mH)    | 0.644 | 1.3 | 0.9 | 5.4 | 0.35 |
| Back EMF constant (volts/rad/sec)|0.2455 | 0.1413 | 0.08 | 0.5730 | 0.0191 |
| Motor inertia (kgm²) | 1340 |6355| 2118 | 21890 | 155 |
| Motor friction coefficient (mNm.s/rad) | 0 |1| 2 | 3 | 4|

| Mechanical system| Load#0| Load#1| Load#2| Load#3| Load#4|
| :--------------: |:-----:| :----:|:-----:| :----:|:-----:|
| Load side friction coefficient (mNm.s/rad)| 0.4 | 0.5 | 0.18 | 0.36 | 0.06 |
| Load inertia (kgm²)            | 1800 | 9000 | 1800 | 36000 | 360 |
| Load torque (rated) (Nm)       | 1.6 | 1.5 | 0.75 | 1.9 | 0.18 |

* There is no gearbox in the system.
* Combined inertia (motor + load) can be used.
* Combined viscous friction (motor + load) can be used.

If you require more information about the motors, please refer to the data sheets:

- Motor #0:

- Motor #1:

- Motor #2:

- Motor #3:

- Motor #4:
