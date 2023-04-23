# Lab Report 2  
  
## Part 1  
## Part 2  
The bug for analysis here is the Array reverses functions (testReverseInPlace and testReversed).  
For the first method, testReverseInPlace, a couple wrong inputs were:  
```
    int[] input3 = {2, 3};
    int[] input4 = {1, 2, 3, 4};
    ArrayExamples.reverseInPlace(input3);  
       
    assertArrayEquals(new int[] {4, 3, 2, 1}, input3);
    ArrayExamples.reverseInPlace(input4);
    assertArrayEquals(new int[] {3, 2}, input4);
```

## Part 3  
