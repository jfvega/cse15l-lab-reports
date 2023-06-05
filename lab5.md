## Lab 5
# Part 1: Debugging Scenerio
1.
![Image]()
![Image]()

**TA Response**
- Thank you for the question. So it looks like here that you are trying to find ListExamples.java anywhere in the students-submission directory. The code looks correctly implemented, you have all they key details down. One thing you need to make sure is write what you are exaclty looking for. If your looking for a specific file type then state the file type. Say I am looking for a .sh file. It should show all the .sh files. Here your code isn't doing that. Take a look again, and see if you can use this idea in your code. 


**Student Response**
- I see. So the bug in my code is in line 11. I am missing .java on the end of ListExamples. The code is looking for a certain type of file and can't find anything because of that simple error. Thank you. 
![Image]()
![Image]()

**All setup**
-To begine working you need to make sure you are in the right directory/repository. This should be the grader-skill-demo2.
![Image]()
-Run using bash to see if grade.sh is working.
![Image]()
-Next you need to open up your contents in grade.sh since that is hwere your bug is.
- Command line: `vim grade.sh`
- Then fix the bug by adding .java to the end of ListExamples on line 11
- Lastly run the code again to see if that fixed the mistake. 
- ![Image]()
