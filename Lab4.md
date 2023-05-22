## Lab Report 4  
  
Start with logging in:
```
ssh cs15lsp23ov@ieng6.ucsd.edu <Enter>
```
This just logged me in remotely into the server. Note: No password was prompted and entered because of the  
ssh keys set up in lab previously.  
The end result image was:  
[!Image](Lab4ScreenShot1.PNG)  

Next, I needed to clone the repository, which was done with the code:  
```
git clone https://github.com/r9sun-ucsd/lab7.git <Enter>
```
The keystrokes were exactly as typed in the code above and resulted in the following output:  
[!Image](Lab4ScreenShot2.PNG)  

Next, I needed to check that the code was broken. The following command was used.  
```
bash test.sh <Enter>
```
This ran the JUnit tester on the code and outputted the following error message, oh no!  
[!Image](Lab4ScreenShot3.PNG)  
  
Due to this, I had to fix the wrong code using the vim text editor. 
```
vim ListExamples.java <Enter>
/index1 
nnnnnnnnn
lllll i <backspace> 2
<esc> :wq
```  
The first line was getting into the vim editor for the file ListExamplesjava.   
The next line that used "/index1" upon launching executed a search of the key phrase index1 because  
that was the error that we were looking for to switch. Upon launching the search, it took me to the  
first instance of index1 popping up in the code, where the next 9 "n" commands were going through all  
the times "index1" popped up in the code to reach the instance of the "index1" that we needed to switch  
to "index2". The next 5 "l" commands were moving right on that line to reach the "1" to replace and delete.  
The "i" command puts vim into edit mode, where backspace and 2 changed "index1" to "index2". Finally, "esc"  
could be called to exit back to normal mode from insert mode, and then the file could be saved and quit with ":wq". 
The code's final result was:  
[!Image](Lab4ScreenShot4.PNG) 
  
From here, we could retest the corrected, fixed code to show the error being gone!  
```
<Up> <Up> <Enter>
```
The up commands were called because they referenced previous commands. Due to us testing the file earlier,  
we can simply go back two commands to rerun the previously run test command. This gives us the new output:  
[!Image](Lab4ScreenShot5.PNG)  
  
The fixed code can now be pushed to my repository.  
```
git add ListExamples.java
git commit
i Whoa!!!! <Escape> :wq
```  
The git add adds the file that should be pushed to the git repository. Since I have edited the  
ListExamples.java code to be correct, I want to push that to my repository. The git commit officially  
sends and pushes the files that were all added with git add. After running git commit, a new screen with  
the vim editor was put on the terminal screen to add a commit message. The "i" entered insert mode so that  
I could add my edit message, which was "Whoa!!!!". <Escape> and ":wq" allowed me to save the commit message  
and finalize sending that commit. That resulted in the following output.  
[!Image](Lab4ScreenShot6.PNG)  
  
Tada! The End (I hope you enjoyed)!
