# Lab Report 4
## Misha Tavera
----- 
  In this weeks lab we focused on using `vim` to develop our skills and eficiency in editing any program. We essentially doing this by using `vim` and it's command-line function of diirectly making edits to a piece of code from the command line. To summarize, `vim` has two modes, normal mode and insert mode. The insert mode essentially allows you to make the edit to the code by typing in any changes, while in the normal mode all keys have some kind of function that help you navigate through any text of code effciently. In this normal mode, there is a long list of what each key can do but for this lab we only used some of the many which I explain below. 


  In the lab we had a code file that contained an error, our task was to edit the code using `vim`. It was only a small error but the focus here was to practice and get familiar with some elements of `vim` and how it can make editing a code file quite simple and fast all from the command line. We were encouraged to go first with our immediate guess to approach the edit based on some basic information we had from lectures/lab. Then, using some provided tips and resources we retry to make the edit with the intention of fewer keystrokes or in a faster manner. 

Going into it my first initial way of going about it was to use `vim` to pull up the code file with the error and (in normal mode) use the 'j' key repeatedly to find the line I was looking for. Then I used the `l` to move my cursor to the right character by character. Using the `i` key to change to insert mode I used `<backspace>` and then typed the my intended change accordingly. What that looked like exactly in keystrokes is: 

`j,j,j,j,j,j,j,j,j,j,j,j,j,j,j,j,j,j,j,j,j,j,j,j,j,j,j,j,j,j,j,j,j,j,j,j,j,j,j,j,j,j,j,l,l,l,l,l,l,l,l,l,l,l,l,i,<backspace>,2 (to make the change ``1`` to ``2`` after 'index'), <esc>, :,w,q, and finally g,i,t, <space>, a,d,d, <enter>, g,i,t, <space> , c,o,m,m,i,t, <space> , -, m, <space> , MESSAGE,<enter>, g,i,t , <space> ,o,r,i,g,i,n, <space> ,m,a,i,n, <enter>` to commit and push all changes to the repository. 
