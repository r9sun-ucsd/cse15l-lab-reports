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
Here's the proof: 
## Part 3  
