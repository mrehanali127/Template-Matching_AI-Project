# Template-Matching_AI-Project
## How to find particular thing in image through AI
## Problem
We are supposed to solve an image processing or pattern recognition problem using our
computational model. e.g, In our case, We are finding the location of a small image
in the bigger image. These images can be any other object or patterns like maps,
tables, windows, and doors, etc.

## Flow of Model
![alt text](https://github.com/mrehanali127/Template-Matching_AI-Project/blob/master/flowchart.PNG?raw=true)

## Computational Model
The following are the steps that we will follow to solve our template matching problem:<br/>
1)Representation:<br/> Images are represented in the form of matrices and these matrices are
filled with the number and these numbers correspond to all the individual pixels of the
image.<br/>
2)Initial Population:<br/> We will randomly select a pre-defined number of points from our
search space or the bigger image. All of these represent the location of our potential
solutions in the bigger image. In the next step, we will be checking how good or bad is
each of these solutions.<br/>
3)Fitness Function:<br/> Our fitness function will take three inputs(Bigger Image, Smaller
Image, and the Initial Population). It will give us the fitness value. This value will tell us how
fit is our potential solution by comparing it with the smaller image. The value will range
between 0 to 1. 1 means 100% match and 0 means 0% or no match etc.<br/>
4)Sorting and Saving the Fittest Solution:<br/> We will sort our potential solutions based on
their fitness value and save the fittest solution of the whole generation. Here we are
artificially selecting the best fit and in the case of the theory of evolution, this was done
naturally by Natural Selection.<br/>
5)CrossOver and Mutation:<br/> After saving the fittest solution from our sorted Array, We will
cross the pairs in our population to create a new population. We will cross 1st solution and
2nd solution, then 2nd solution and 3rd solution,…, then lastly 2nd last solution with the
last solution in our ranked population. Here a new population will be generated.<br/>
By doing CrossOver and Mutation our new population is actually being evolved from the
older population. This same concept of evolution was given in our Evolutionary theory for
living species.<br/>
6) After creating a new population, We will jump on Step 3 of fitness calculation and
continue this process until a certain threshold is met. A threshold hold could be a matching
percentage based on the output of fitness function or a particular number of generations.<br/>

