# Lab 5 Report
## Part 1 – Debugging Scenario

Here is the question student has regarding to the bug they have:

![question 1](https://github.com/jayden789/cse15l-lab-reports/assets/112384009/a67a8b2a-2acf-4cb1-a2ef-63f852982a73)


The TA examined asked for the codes of grade.sh because it looks like the bug is from that file
Here the code inside `grade.sh`

![grade-file](https://github.com/jayden789/cse15l-lab-reports/assets/112384009/ce75c31f-5b98-40ba-bfdf-9262f3112497)


After considering, the TA recommended to change "PATH" variable to "path"

![initial fix](https://github.com/jayden789/cse15l-lab-reports/assets/112384009/00fd7e65-14c3-4cdc-8fb0-525c17ffe0cf)


What shown on the terminal after changing "PATH" to "path"

![inital-ter](https://github.com/jayden789/cse15l-lab-reports/assets/112384009/39015628-f1b2-4250-910a-39ced4643530)

The student asked for help as the test failed because the `ListExamples.java` was cloned from
the corrected implementation. So they expected it should have passed.

The URL where `ListExamplesjava` file is cloned and tested on
https://github.com/ucsd-cse15l-f22/list-methods-corrected.git

The implementation inside `ListExamplesjava` file

![correct-j](https://github.com/jayden789/cse15l-lab-reports/assets/112384009/6b224520-81de-45bd-a673-4e40ba682b28)

The TA checked and asked for photo of hierrachy of directories

![directory](https://github.com/jayden789/cse15l-lab-reports/assets/112384009/a5c736a5-b6be-4eda-b30f-a601345effd9)

The TA asked for a look at implementation of `ListExamples.java` outside the student-submission
This file contains the bug inside the merge() method

![buggy-j](https://github.com/jayden789/cse15l-lab-reports/assets/112384009/f6e281fc-dda1-43d8-8ce7-cc38332dbe30)


The TA suggested to include `cd grading-area` inside `grade.sh` script to change the directory
so the corrected `ListExamples.java` will be tested

![final-fix](https://github.com/jayden789/cse15l-lab-reports/assets/112384009/c0e14a41-d68f-4a93-9b54-f9fef7ba5799)

The result student got after updating the `grade.sh` file

![final-ter](https://github.com/jayden789/cse15l-lab-reports/assets/112384009/2d6a6315-6bed-494a-be6d-c823e0c20d25)

Overall,
the file & directory structure needed: working directory: inside `grading-area`
( Student need to change directory to grading-area if that is not the current directory)
File needed: `hamcrest-core-1.3.jar`, `junit-4.13.2.jar`, `TestListExamples`, `ListExamples.java`

A description of what to edit to fix the bug:
There are two bugs, one in `grade.sh`that **PATH** cannot be used as a varible (lower-case will works).
The other bug is inside merge method of `ListExamples.java` that **index1** should be changed to **index2**

# Part 2 – Reflection

From the second half of this quarter, I have learned how to write bash script and run java files from the script.
That is the main takaway from the this course.
The other thing I wish I could have more practice on would be File object processing, standard output and error redirection,
as long as some other commands that were covered in class but we have not used in the lab.

Overall, for a 10-week course, this is still a lot that I have gain compared the first day of class.
All the tutors and TA are helpful and friendly. I also made friend with one!
