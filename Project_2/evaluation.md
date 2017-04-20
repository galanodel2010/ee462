## Evaluation Guideline for Project #2

The project will be evaluated using the following guideline:

**Number of Commits:25%:** The number of edits of your project files as seen from the contributors list. For example, if you start making your project in the last few days, you’ll get no credit. If you start early and continue editing your files, you’ll get full credit. The project topics are not easy, so this is a way to encourage you to start early and work regularly.

**Report Quality:15%:** Text explaining your design decisions, quality of your figures, citing relevant studies and your conclusion section.

**Technical Level (Part-I&II):60%:** The detail level of your designs (see requirements above), and the accuracy of your calculations.

**Technical Level (Part-III Bonus):15%:**

## Number of Commits:

In this project the expected number of commits on different days is 10. Each days you made at least one commit is 2 points (saturating at 20 points). Thus, if you made 4 commits at 3 days, you'll get 6 points. The following rules apply:

- Your commit has to be a meaningful, and considerable amount of change has to be made compared to the previous version. For example, just changing a few words in your report is not a meaningful commit.

- Number of days that you committed will be evaluated by common sense. For example, a commit at 23:58 and another commit at 00:02 will still count as one.

- Do not try to find a workaround. Just spend time on your project, and improve your models regularly and it should be fine.

You'll get 5 points from the content of your commit messages. You are supposed to write clear and explanatory commit messages, listing what  specific improvements that you made in that version. Please have a look at the following links:

- [Writing Good Commit Messages](https://vip.wordpress.com/documentation/commit-messages/)
- [What makes a good commit message?](https://hackernoon.com/what-makes-a-good-commit-message-995d23687ad#.o13dxmu3u)

![](https://imgs.xkcd.com/comics/git_commit.png)

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

**Part-A Preliminary Design**

- Enough theoretical background is presented to choose the DC-link filter elements. (4pts)
- Enough results are given to prove that 1% ripple condition is satisfied. (3pts)
- The switching frequency is chosen properly and the chosen value is reasonable. (3pts)

**Part B: Modeling and Simulation**

- The designed PWM system is capable of applying four-quadrant operation, and these modes are clearly demonstrated (both with simulation results and with theoretical information). (4pts)
- The system successfully driven with 0.6 duty cycle (with constant DC voltage), and the required waveforms are presented. (3pts)
- The system is combined with the diode-rectifier, and the change in drive characteristics is well presented with enough comments. (4pts)

**Part C: Open Loop Control**

- Forward Motoring at Rated Speed:
    - Required duty cycle for rated speed is calculated correctly. (3pts)
    - The required plots are presented with additional comments. (3pts)

- Rated Speed to Half Speed Step Response:
    - Required duty cycle for 0.5 rated speed is calculated correctly. (3pts)
    - Change in the DC-link voltage and the direction of the power flow during transient is presented. (3pts)
    - Comments on the operation mode during the transient. (3pts)

**Part D: Dynamic Braking**

- Braking is applied to the motor when it is running at the steady-state speed and the required plots are presented with additional comments. (3pts)
- The methodology of choosing the braking resistor is presented. (3pts)
- The braking chopper circuit is implemented. (3pts)

**Part E: Closed Loop Control**

- Some background information about PID controllers are presented. (3pts)
- Current controller is implemented, and the acceleration transient is presented with required plots. (3pts)
- Information about the selection of PID controller gains is presented. (3pts)
- Hysteresis current controller is presented with required plots. (3pts)
- Two methods are compared listing the advantages and disadvantages of each system. (3pts)

**Part F: Speed Controller**

- Speed controller is implemented with some background information. (3pts)
- The system accelerated from standstill to rated speed and the plots are given to prove the operation with enough comments. (2pts)
- The system is accelerated and decelerated with within the maximum limits defined. (2pts)
- Jerk limitation is implemented in the control loop. (2pts)

**Part G: Component Selection**

- Reasonings for choosing the suitable power electronics is presented. (2pts)
- Commercially available components are investigated and a proper device is chosen for the transistors and the reasons behind the choice are explained. (2pts)
 - Commercially available components are investigated and a proper device is chosen for the rectifying diodes and the reasons behind the choice is explained. (2pts)
