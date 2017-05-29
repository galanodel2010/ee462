## Evaluation Guideline for Project #3

The project will be evaluated using the following guideline:

**Number of Commits:25%:** The number of edits of your project files as seen from the contributors list. For example, if you start making your project in the last few days, you’ll get no credit. If you start early and continue editing your files, you’ll get full credit. The project topics are not easy, so this is a way to encourage you to start early and work regularly.

**Report Quality:15%:** Text explaining your design decisions, quality of your figures, citing relevant studies and your conclusion section.

**Technical Level (Part-I&II):60%:** The detail level of your designs (see requirements above), and the accuracy of your calculations.

**Technical Level (Part-III Bonus):20%:**

## Number of Commits:

In this project the expected number of commits on different days is **10**. Each days you made at least one commit is 2 points (saturating at 20 points). You'll get 5 points from the content of your commit messages. You are supposed to write clear and explanatory commit messages, listing what  specific improvements that you made in that version.

## Report Quality:

You report quality will be evaluated using the following criteria:

- The report has a separate title page (1pts*)
- The report has a table of contents page (1pts*)
- The report has an introduction section that briefly explains the content and the aims of the report (2pts)
- The report organized properly with clear sections and subsections (1pts)
- All figures and tables have proper captions (2pts)
- The graphs have proper axes labels and font size of labels is adequate (2pts)
- The graphs does not have the [default black background](people.uncw.edu/hermanr/mat361/Printing%20Simulink%20Scope%20Image.pdf), and line colors are distinguishable (1pts)
- No grammar/spelling errors and very well-written report (hint: use spell-check) (2pts)
- The report has a conclusion section that summarizes what have been achieved (2pts)
- The report has a [bibliography](http://www.plagiarism.org/citing-sources/whats-a-bibliography/) section and all the external sources [have been cited properly](http://libguides.mit.edu/citing). Note that, this is for formatting of the citations. Any [plagiarism](http://www.plagiarism.org/plagiarism-101/what-is-plagiarism) will not be tolerated. (1pts)

(*) These points do not apply for reports written in Markdown. For those reports you"ll get the points automatically.

## Level of Information:

For this project following will be checked in your reports and in your models:

**Part-A Motor Characterization**

- Torque-speed characteristics plot (2pts)
- Starting torque, pull-out torque and the rated torque values are calculated (2pts)
- Torque-speed curves at 4 different Constant V/f values (2pts)

**Part B: Drive Proposition**

- Power-stage topology is well explained with enough comments (2pts)
- Required measurements are well explained (2pts)
- Components are properly chosen and the analytical calculations and reasonng are presented (3pts)
-  Closed-loop control block diagram is presented and explained (2pts)

**Part C: Open Loop V/f Control**

- Plots for starting from standstill with rated voltage (3pts)
- Plots for Starting from standstill with half of the rated voltage (3pts)
- Comparison of these two cases and the analytical calculations (4pts)
- Analytical calculations for 0.1 pu speed and simulation results (5pts)

**Part D: Closed Loop Control**

Verification of the closed loop operation with tests:

- Starting current is limited at startup (3pts)
- Speed regulation (from full load to no load) (3pts)
- Speed bandwidth (from positive to negative speed) (3pts)
- Flux weakening mode of operation (3pts)

- Comments about all operating modes and self-criticism about the performance of the drive (3pts)

**Part E: Component Selection and Verification**

- Selection of components for power semiconductor devices (3pts)
- Verification of safe operation of these selection using your previous plots (3pts)

**Part F: Loss characterization and efficiency calculation**

- Calculation of losses using component datasheets (3pts)
- Calculation of the overall efficiency of the motor drive system (3pts)
- General comments about the effciency and advices to get a higher efficiency (3pts)

**Part G: Field oriented control (BONUS)**

- Brief summary about the field oriented control  (5pts)
- FOC is implemented and the id, iq values are calculated (3pts)
- Plots for starting from stationary to rated speed (3pts)
- Performance comparison with V/f control (3pts)
- Speed bandwidth test results (3pts)
- Comparison of speed bandwidth with the V/f control (3pts)
