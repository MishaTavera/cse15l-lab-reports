# LabReport 3
## Misha Tavera

--- 
## Part 1: Bugs

### Failure-Inducing Input:

``` 
   @Test
    public void testAverageWithoutLowestMultiRepeat(){
    double [] input1= {1,1,1,2,3,4};
    assertEquals(2.2,ArrayExamples.averageWithoutLowest(input1),0.0001);
 }
```

### Passing Tests:
```
   @Test
  public void testAverageWithoutLowest3(){
    double [] input1= {1};
    assertEquals(0,ArrayExamples.averageWithoutLowest(input1),0.0001);
  }
   @Test
  public void testAverageWithoutLowest4(){
    double [] input1= {1,2};
    assertEquals(2,ArrayExamples.averageWithoutLowest(input1),0.0001);
  }
     @Test
  public void testAverageWithoutLowest5(){
    double [] input1= {1.0,2.0,3.0};
    assertEquals(2.5,ArrayExamples.averageWithoutLowest(input1),0.0001);
  }
```
### Before Code: 
```  // Averages the numbers in the array (takes the mean), but leaves out the
  // lowest number when calculating. Returns 0 if there are no elements or just
  // 1 element in the array
  static double averageWithoutLowest(double[] arr) {
    if(arr.length < 2) { return 0.0; }
    double lowest = arr[0];
    for(double num: arr) {
      if(num < lowest) { lowest = num; }
    }
    double sum = 0;
    for(double num: arr) {
      if(num != lowest) { sum += num; }
    }
    return sum / (arr.length - 1);
  }
````
![failed](failure-inducing.png)

![firstpassed](passedTests.png)

### After Code: 


Provide:



A failure-inducing input for the buggy program, as a JUnit test and any associated code (write it as a code block in Markdown)
An input that doesn't induce a failure, as a JUnit test and any associated code (write it as a code block in Markdown)
The symptom, as the output of running the tests (provide it as a screenshot of running JUnit with at least the two inputs above)
The bug, as the before-and-after code change required to fix it (as two code blocks in Markdown)


## Part 2: Researching Commands

