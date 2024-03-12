# Lab Report 5
## Misha Tavera
----- 

## Part 1: Debugging Scenario 

---
**EsStemDiscussion**
> Misha: Hi, I am working on the autograding script from lab. I am having trouble getting it to work properly. I found there to be some kind of bug in my bash script but I can't seem to find it. The script works for most of the repositories we have to test our grader only it does not seem to work for the one that is supposed to be correct. From the output I believe it has something to do the last lines of my bash script where it calculates the student's score. I have tried changing the fields for `awk` but that doesn't seem to help, can anyone please help?
>
>  My grading script: ![buggygradingscript](buggygrader.png)
>
> My command and it's buggy output: ![bugoutput](buggraderouput.png)
>
>
> > TA: Looking at your output what is being printed that shouldn't be and where is this coming from? Hint look at the actual output in the `grading area`. How is the output different from other repositories that do pass? And how should this be reflected in your bash grading script?
> >
> > >Misha: Thank you this was very helpful I see where I went wrong. My bug is in that my `grade.sh` the lines to print out a score are hard coded. By looking in `junit-output.txt`, which is where the jUnit output of my `TestListExamples.java` is redirected, I see that the bash scrip is only set up to successfully print and score the repositories that had some kind of error in them. To correct this I will add to my bash script to account for not only the repositories with errors but the ones that pass and print a different output in `junit-output.txt`.
> > >
> > >My `junit-output.txt` of a repository with errors: ![error](failingrepo.png)
> > >My `junit-output.txt` of the passing repository: ![passing](passingrepo.png)
> > 
---





-----

## Part 2: Reflection

In general I enjoyed learning about all the topics we discussed but somethings that stood out to me is when we learned how to write a bash grading script. We did this in class and in lab in week 6 and I liked learning about it because I feel like it is something that definetly correlated to something in my life. Before I did not know or think about how any work was graded but now I do and even learned how to write one myself. I learned the actual specific like what goes into the actual grading bash script but in general I also just liked learning about kind of what goes on behind the scenes of something I hadn't thought of before. Especially because having taken other cse courses I have definetly interacted with grading scripts before being used on my own programming, so I thought it was cool to learn about how something like that works and is built. 
