## Lab Report 4
  

Actual Code:  
```
vim ListExamples.java
</> <i> <n> <d> <e> <x> <1>  
<n> <n> <n> <n> <n> <n> <n> <n> <n> 
<l> <l> <l> <l> <l> <i> <backspace> <2>
<esc> <:> <w> <q>
```
The first line that used "/index1" upon launching executed a search of the key phrase index1 because  
that was the error that we were looking for to switch. Upon launching the search, it took me to the  
first instance of index1 popping up in the code, where the next 9 "n" commands were going through all  
the times "index1" popped up in the code to reach the instance of the "index1" that we needed to switch  
to "index2". The next 5 "l" commands were moving right on that line to reach the "1" to replace and delete.  
The "i" command puts vim into edit mode, where backspace and 2 changed "index1" to "index2". Finally, "esc"  
could be called to exit back to normal mode from insert mode, and then the file could be saved and quit with ":wq".  
  

