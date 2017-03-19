## Evaluation Guideline for Project #1

The project will be evaluated using the following guideline:

**Number of Commits:25%:** The number of edits of your project files as seen from the contributors list. For example, if you start making your project in the last few days, you’ll get no credit. If you start early and continue editing your files, you’ll get full credit. The project topics are not easy, so this is a way to encourage you to start early and work regularly.

**Report Quality:25%:** Text explaining your design decisions, quality of your figures, citing relevant studies and your conclusion section.

**Technical Level of Information:50%:** The detail level of your designs (see requirements above), and the accuracy of your calculations.

## Number of Commits:

In this project the expected number of commits on different days is 5. Each days you made at least one commit is 4 points (saturating at 20 points). Thus, if you made 4 commits at 2 days, you'll get 10 points. The following rules apply:

- Your commit has be a meaningful, and considerable amount of change has to be made to the previous version. For example, just changing a few words in your report is not a meaningful commit.

- Number of days that you committed will be evaluated by common sense. For example, a commit at 23:58 and another commit at 00:02 will still count as one.

- Do not try to find a workaround. Just spend time on your project, and improve your models regularly and it should be fine.

You'll get 5 points from the content of your commit messages. You are supposed to write clear and explanatory commit messages, listing what  specific improvements that you made in that version. Please have a look at the following links:

- [Writing Good Commit Messages](https://vip.wordpress.com/documentation/commit-messages/)
- [What makes a good commit message?](https://hackernoon.com/what-makes-a-good-commit-message-995d23687ad#.o13dxmu3u)

![](https://imgs.xkcd.com/comics/git_commit.png)

## Report Quality:

You report quality will be evaluated using the following criteria:

- The report has a separate title page (2pts*)
- The report has a table of contents page (2pts*)
- The report has an introduction section that briefly explains the content of the report (3pts)
- The report organized properly with clear sections and subsections (2pts)
- All figures and tables have proper captions (3pts)
- The graphs have proper axes labels and font size of labels is adequate (3pts)
- The graphs does not have the [default black background](people.uncw.edu/hermanr/mat361/Printing%20Simulink%20Scope%20Image.pdf), and line colors are distinguishable (2pts)
- No grammar/spelling errors and very well-written report (hint: for a start use spell-check) (3pts)
- The report has a conclusion section that summarizes what have been done (3pts)
- The report has a [bibliography](http://www.plagiarism.org/citing-sources/whats-a-bibliography/) section and all the external sources [have been cited properly](http://libguides.mit.edu/citing). Note that, this is for formatting of the citations. Any [plagiarism](http://www.plagiarism.org/plagiarism-101/what-is-plagiarism) will not be tolerated. (2pts)

(*) These points do not apply for reports written in Markdown. For those reports you"ll get the points automatically.

## Level of Information:

For this project following will be checked in your reports and in your models:

- All three models are running properly without errors (3pts)
- All three models are consistent with each other. (3pts)

**Part-1**
- Analysis and results (3pts)
- Comments (10 pts)
    - General comments on the the operation
    - How does the speed and the torque of the motor changes?
    - What is the effect of the inertia on the acceleration. Propose a method to determine the mechanical time constant and electrical time constant.
    - Comment on the difference of motor speed and load speed. What is the effect of the shaft stiffness in the transient response of the model?
    - How does the efficiency changes with speed, Why?

**Part-2**
- Analysis and results (3pts)
- Comments (10 pts)
    - General comments on the the operation
    - How does the speed and the torque of the motor changes?
    - Comment on the direction of power, and mode of operation. What kind of practical issues you will face in the practical implementation of this?
    - What can you do to implement this kind of operation, if you only have a uni-directional power supply? 

**Part-3**
- Analysis and results (3pts)
- Comments (10 pts)
    - General comments on the the operation
    - Comment on the time it takes to accelerate with the results you obtained in Part-1.
    - Roughly estimate and compare the energy dissipated (in Joules) in the armature resistance(Ra) in Part-1 and Part-3 during the acceleration period. Comment on the effect of these two starting methods on the temperature rise of the motor.
    - Propose a method for soft-starting the motor practically, if you didn't have an ideal controllable voltage source.

**Model Quality**: (5pts)

Your model files will be evaluated in the following ways: 

- Model filenames are proper and self-explanatory (2 pts)
- Blocks in the model are [neatly arranged](http://blogs.mathworks.com/pick/2014/04/25/clean-up-your-simulink-model/) and all signals are labeled for easy debugging (3pts)
