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
  
Due to this, I had to fix 
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
[!Image](Lab4ScreenShot1.PNG) 
  

