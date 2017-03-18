## Project 1 - Data-Sheets

## How to choose the motor-load combination?

The motor parameters will be assigned randomly, based on the last digit of your student number. For example if your student number is 1244839, then take the modulus 5 of the last digit:

mod-5 (9) = 4

Then you need to use the parameters of the Motor#4 for your project.

## Motor Data-Sheet

In this project, you will be all using small permanent-magnet brush DC motors from [Maxon Motors](http://www.maxonmotor.com) and [Moog](http://www.moog.com/)

Please refer to the data according to the number you are assigned to.

| DC motor| Motor#0| Motor#1| Motor#2| Motor#3| Motor#4|
| :-----: |:-----:| :----:|:-----:| :----:|:-----:|
| Rated armature voltage (V) | 70 | 48 | 24 | 90 | 12 |
| Rated output power (W)| 250 | 192 | 121 | 359 | 26 |
| Rated speed (rpm)  | 2490 | 3226 | 2700 | 1517 | 4700 |
| Armature resistance (Ω)    | 1.41 | 0.7 | 0.43 | 1.45 | 0.6 |
| Armature inductance (mH)    | 0.644 | 1.3 | 0.9 | 5.4 | 0.35 |
| Back EMF constant (volts/rad/sec)|0.2455 | 0.1413 | 0.08 | 0.5730 | 0.0191 |
| Motor inertia (gcm²) | 1340 |6355| 2118 | 21890 | 155 |

| Mechanical system| Load#0| Load#1| Load#2| Load#3| Load#4|
| :--------------: |:-----:| :----:|:-----:| :----:|:-----:|
| Gearbox ratio (N1:N2)         | 2:1 | 3:1 | 2:1 | 1:1 | 4:1 |
| Load side friction coefficient (mNm.s/rad)| 0.4 | 0.5 | 0.18 | 0.36 | 0.06 |
| Motor Shaft stiffness (Nm/rad)   | 15 | 8 | 7.5 | 36 | 1.2 |
| Load inertia (gcm²)            | 1800 | 9000 | 1800 | 36000 | 360 |
| Load torque (Constant) (Nm)       | 1.6 | 1.5 | 0.75 | 1.9 | 0.18 |

(*) Assume the gearbox is lossless.
(*) No coulomb friction, only viscous friction


If you require more information about the motors, please refer to the data sheets:

- Motor #0: http://www.maxonmotor.com/maxon/view/category/motor?target=filter&filterCategory=DC-max

RE 65 Ø65 mm,
Part number 353301

- Motor #1: [Moog C42-L50-10](www.peromatic.ch/fileadmin/user_upload/PDF/MOOG/DC_MOTOREN/C42.pdf)

- Motor #2: [Moog C34-L60-10](http://www.moog.com/content/dam/moog/literature/MCG/moc23series.pdf)

- Motor #3: [Moog C42-L90-30](www.peromatic.ch/fileadmin/user_upload/PDF/MOOG/DC_MOTOREN/C42.pdf)

- Motor #4:  [Moog C23-L33-10](http://www.moog.com/content/dam/moog/literature/MCG/moc23series.pdf)


<!--- Diger Motor Datalari
http://www.moog.com/literature/MCG/moc23series.pdf
http://w3app.siemens.com/mcms/infocenter/dokumentencenter/ld/Documentsu20Catalogs/dc-motor/da12-2008-en.pdf
http://ecatalog.weg.net/files/wegnet/WEG-specification-of-electric-motors-50039409-manual-english.pdf
http://www.maxonmotor.com/maxon/view/category/motor?target=filter&filterCategory=DC-max
http://www.kollmorgen.com/en-us/products/motors/brush-dc/permanent-magnet-dc-pmdc/
http://www.moog.com/literature/MCG/moc23series.pdf
-->
