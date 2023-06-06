# Lab Report 5  
## Debugging Help  
  
Mock Post:
What environment are you using (computer, operating system, web browser, terminal/editor, and so on)?
I am currently attempting to do my grading script. I am currently using VS Code on my own computer, which is a Windows, trying to run my grade.sh script in bash!  

Detail the symptom you're seeing. Be specific; include both what you're seeing and what you expected to see instead. Screenshots are great, copy-pasted terminal output is also great. Avoid saying “it doesn't work”.  
The error output here is:  
[!Image](Lab5_Error_Message.PNG)  
The code should instead run properly, and return that all 5 tests were correct with 5/5 being returned.  

Detail the failure-inducing input and context. That might mean any or all of the command you're running, a test case, command-line arguments, working directory, even the last few commands you ran. Do your best to provide as much context as you can.  
I was just running my grade.sh file when this output happened, with the context shown in the screenshot given above. I was trying to test the correct output for my grading script on one of the repositories that should've returned a good score, but I got the error message as shown above.  
  
Mock TA Response:
Hello! Do you mind telling me what specific code changed, and if I could see your code for your grade.sh file and your GradeServer.java file to see if it is in the correct state currently. That being said, it appears that either your GradeServer or bash script is having an issue understanding a specific parameter, so look at the code that parses in specific arguments, files, and URLS maybe to see the issue.

  
## Reflection  
One of the things I enjoyed learning about this quarter was the creation of our own grading scripts. While definitely simplified, and one of the harder, more tedious labs, it was cool to see the real applications of this class. During the lab sections involving the autograder, I learned a bit more about bash and reviewed some commands like grep and whatnot, and how to apply them in bash, to run the autograder script that would 
