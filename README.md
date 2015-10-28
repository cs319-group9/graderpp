# graderpp
Grader++ is a code evaluation system we plan to develop in aid to the instructors and teaching assistants. Most of the time, instructor’s method of grading student’s codes involves steps that can be automated by a software system. For example, a instructor firstly compiles student’s code and checks if there is a compilation error, afterwards, he/she checks if the code has memory leaks, and tries a few testcases and compares output to solution. Steps like this can be easily automated by a software and takes a lot time of the instructors grading code submissions. 

There is problems automating the this kind of tasks like that. Students might submit dangerous codes which can be caught by instructor by looking at the code, automating this process and handling dangerous codes is difficult. We plan to make grader++ secure by using technologies like containers and extendible, since every course, even homework, needs different evaluation steps and fast, since a course could be taken by a lot students and most of the students submit their code at last minute and it will create a lot of load on the system.

Grader++ has two parts: Core part and UI part. Core part will be an extendible system composed of evaluators, evalating submissions concurrently. UI part will give ability to instructors to add homeworks to the system and students to submit their code. Core part will be a restful api server, accepting task descriptions and submissions. UI part will interact core part through http requests and will have a web frontend in which instructors and students could interact core part with ease. Seperating core part from UI will enable us to easily extend our system and will enable us to use more than one server, so that UI part wil be accessible under heavy load.



