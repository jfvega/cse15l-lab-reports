## Lab 5
# Part 1: Debugging Scenerio

![Image](Screenshot 2023-06-05 at 4.17.24 PM.png)
![Image](Screenshot 2023-06-05 at 4.17.38 PM.png)

**TA Response**
- Thank you for the question. So it looks like here that you are trying to find ListExamples.java anywhere in the students-submission directory. The code looks correctly implemented, you have all they key details down. One thing you need to make sure is write what you are exaclty looking for. If your looking for a specific file type then state the file type. Say I am looking for a .sh file. It should show all the .sh files. Here your code isn't doing that. Take a look again, and see if you can use this idea in your code. 


**Student Response**
- I see. So the bug in my code is in line 11. I am missing .java on the end of ListExamples. The code is looking for a certain type of file and can't find anything because of that simple error. Thank you. 
![Image](Screenshot 2023-06-05 at 4.27.45 PM.png)
![Image](Screenshot 2023-06-05 at 4.27.12 PM.png)

**All setup**

-To begin working you need to make sure you are in the right directory/repository. This should be the grader-skill-demo2.
![Image](Screenshot 2023-06-05 at 4.29.47 PM.png)
-Run using bash to see if grade.sh is working.
![Image](Screenshot 2023-06-05 at 4.38.42 PM.png)
-Next you need to open up your contents in grade.sh since that is hwere your bug is.
- Command line: `vim grade.sh`
- Then fix the bug by adding .java to the end of ListExamples on line 11
![Image](Screenshot 2023-06-05 at 4.27.45 PM.png)
- Lastly run the code again to see if that fixed the mistake. 
![Image](Screenshot 2023-06-05 at 4.27.12 PM.png)
