# Lab Report 2  
  
## Part 1  
## Part 2  
The bug for analysis here is the Array reverses functions (testReverseInPlace and testReversed).  
For the first method, testReverseInPlace, a couple wrong inputs were:  
```
    int[] input3 = {2, 3};  
    ArrayExamples.reverseInPlace(input3);  
    assertArrayEquals(new int[] {3, 2}, input3);  
      
    int[] input4 = {1, 2, 3, 4};
    ArrayExamples.reverseInPlace(input4);
    assertArrayEquals(new int[] {4, 3, 2, 1}, input4);
```  
However, it did also work for some inputs like:  
```
    int[] input2 = {};
    ArrayExamples.reverseInPlace(input2);
    assertArrayEquals(new int[] {}, input2);
```  
Here's the proof: (Note how the first two tests, the default and my added test work as no error message popped up then)    
![Image](testReverseInPlaceFailure1.PNG)  
![Image](testReverseInPlaceFailure2.PNG)    

So what went wrong?  
It was an issue of copying the data into the array we also had the data in. This means that data in earlier elements data were lost when  
they were overriden and copied over by elements from the end of the array. This means that only number palindromes would've copied properly.  

Before Code:  
![Image](testReverseInPlaceBefore.PNG)  
After Code:  
![Image](testReverseInPlaceAfter.PNG)  

This temp solution works because it stores the original array in a separate, unchanging entity. This means we can safely and reliably  
copy the data over from the temp array into the original array to reverse the original array with the correct data.  
  
## Part 3  
