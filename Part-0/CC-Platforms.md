Part 0 Episode 2/3: Competitive Coding Platforms
=====

There are a variety of platforms that you can use to practise questions and take part in contests. 

We will look at some of the popular and reliable ones:

Codeforces
-----
__Codeforces__ is one of the or if not the most popular website for competitive programming for a variety of reasons including its active community, clean and minimalist UI and interesting problem statements.

__Problems__ are the basic questions that are asked during a contest. They consists of a problem statement followed by input constraints and finally sample test cases. Here is an [example](https://codeforces.com/problemset/problem/4/A) problem.

__Contests__ consits of multiple problems ranging anywhere from 5 to 8 problems (mostly) in a generally increasing sense of difficulty, with each problem being assigned a certain number of points in direct correlation with it's difficulty level.

As time passes during a contest, each problem loses points at the rate of __n/250__ points per minute where **n** is the original value of that problem.

So for instance, if a problem was worth 500 points then:

+ 1 min into the contest - 498 points
+ 2 min into the contest - 496 points
+ 3 min into the contest - 494 points

Your rank is determined by the cumulative sum of the points of all problems you have solved.

When you submited a solution to a task, it is generally run against test cases which were prepared by the contest author. These are called **pre-tests** and they are run during the contests. Passing pre-tests does **not** gurantee the corectness of your solution as there are **system tests** that your code will be run against after the contest has finished. Only upon passing system tests will you be awarded points for that task.

Each submission of yours will contain a verdict indicating how successful it was and you can find a small summary of the verdicts here:

1. Accepted (AC):<br>All tests cases passed and points are awarded.
   
2. Wrong Answer (WA):<br>Your solution produced the wrong answer on a certain test case and hence was not accepted. There is generally no partial marking on Codeforces so **0** points will be awareded for a WA.

3. Runtime Error (RTE):<br>Your code failed during runtime due to an error such as division by 0 or accessing an out of bounds element on an array.
   
4. Time Limit Exceeded (TLE):<br>Your code did not produce the correct answer within the time constraints set by the problem statement. You will need to optimise your code for it to pass.
   
5. Memory Limit Exceeded (MLE):<br>Just like the TLE, your solution tries to use more memory than the constraints set by the question.
   
6. Compilation Error (CE):<br>Your code failed to compile on the judging system. Make sure there are no syntax errors and you have chosen the right language for compilation when you submitted your solution.
   
7. Pretests Passed:<br>As mentioned above, your code has passed __only__ the pretests for the given task. Points will only be awarded once your code also passes the system tests which you __must__ note are generally more rigorous and can cause your program to fail if it is not efficient enough.
   
8. Hacked:<br>If your solution was hacked, it means that someone was able to come up with a test case that was able to break the logic of your solution. To be eligible to hack someone, you must __lock__ your solution which is possible only after you have successfully solved it during the contest. Note that locking a problem means that if someone else hacks your solution, you **will not** be able to resubmit another solution.

Rating System
-----
One may consider three major divisions in Codeforces in which contests take place:

1. Div 3: Rated for < 1600 rating participants
2. Div 2: Rated for < 2100 rating participants
3. Div 1: Rated for >= 2100 rating participants