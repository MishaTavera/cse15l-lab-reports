# LabReport 3
## Misha Tavera

--- 
## Part 1: Bugs

Failure-Inducing Input:


![failed](.jpg)
``` 
   @Test
    public void testAverageWithoutLowestMultiRepeat(){
    double [] input1= {1,1,1,2,3,4};
    assertEquals(2.2,ArrayExamples.averageWithoutLowest(input1),0.0001);
 }
```

Provide:



A failure-inducing input for the buggy program, as a JUnit test and any associated code (write it as a code block in Markdown)
An input that doesn't induce a failure, as a JUnit test and any associated code (write it as a code block in Markdown)
The symptom, as the output of running the tests (provide it as a screenshot of running JUnit with at least the two inputs above)
The bug, as the before-and-after code change required to fix it (as two code blocks in Markdown)


## Part 2: Researching Commands

