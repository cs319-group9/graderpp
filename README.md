# graderpp
![logo](https://raw.githubusercontent.com/cs319-group9/graderppWeb/master/graderppSamples/10x9b3c.jpg)

Grader++ is a code evaluation system we plan to develop in aid to the instructors and teaching assistants. Most of the time, instructor’s method of grading students' codes involves steps that can be automated by a software system. For example, an instructor firstly compiles student’s code and checks whether there is a compilation error, then he/she proceeds by checking if the code has memory leaks, and tries a few testcases and compares output with student's solution. Steps like these can be easily automated by a software and reduces the time it takes for instructors to grade code submissions. 

##Samples from user interface:

 Define a new programming task to a course: (by an Instructor)
![Define a new task] (https://github.com/cs319-group9/graderppWeb/raw/master/graderppSamples/Selection_092.png)

Submit code files to a task: (by a Student)
![Submit code files to a task] (https://github.com/cs319-group9/graderppWeb/raw/master/graderppSamples/Selection_093.png)

View to current assignments (by a Student)
![View to current assignments (by a Student)] (https://github.com/cs319-group9/graderppWeb/raw/master/graderppSamples/Selection_094.png)

##More:

There are problems automating these kinds of tasks. Students might submit malicious codes which can be caught by instructor by scrutinizing the code. Automating this process and handling dangerous codes is difficult. We plan to make grader++ secure by using technologies like containers. Also we will make it extendible, since every course, and even individual homeworks, needs different evaluation steps. Another planned capability for our system is working fast even under a huge work load, because (for example) a course could be taken by a lot of students, and it is possible that a significant amount of students will submit their code at the last minute and it will create a lot of load on the system. In this kind of situation, system should be able to handle evaluating process very efficiently so that students can see the analysis of their code.

Grader++ has two parts: Core part and UI part. Core part will be an extendible system composed of evaluators, evalating submissions concurrently. UI part will give ability to instructors to add homeworks to the system and students to submit their code. Core part will be a restful api server, accepting task descriptions and submissions. UI part will interact core part through http requests and will have a web frontend in which instructors and students could interact core part with ease. Seperating core part from UI will enable us to easily extend our system and will enable us to use more than one server, so that UI part wil be accessible under heavy load.



