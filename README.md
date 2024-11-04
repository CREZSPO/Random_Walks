# :chart_with_downwards_trend: Random Walks :chart_with_downwards_trend: 
A random walk visualization

In mathematics, a random walk, sometimes known as a drunkard's walk, is a stochastic process that describes a path that consists of a succession of random steps on some mathematical space. [1](https://en.wikipedia.org/wiki/Random_walk)
# Problematic 
Imagine we walk to the Empire State building, we play a game with a friend. We throw a dice a 100 times. If it's 1 or 2 we go down a floor/step , if it's 3,4 or 5 we go one step up, if it's a 6 we throw the dice again walking up the resulting number of steps. We can't go below 0 and we can be a little bit clumsy and have a 0.1% of falling down the staris meaning that we would've to restart to step 0. Finally we bet on our friend that we'll make it to step 60 

We have to solve the million-dollar problem: _What are the odds that you'll reach 60 steps high on the Empire State Building?_
For this basically, we want to know about the end points of all the random walks that we will simulate. These end points have a certain distribution that we can visualize with a histogram, but before that I simulated 20 random walks

![download](https://github.com/user-attachments/assets/55d7334f-e5b3-4072-b664-623e9dca6dc5)

Then we can proced to simulate 500 random walks and set them into an histogram.

![hist](https://github.com/user-attachments/assets/1e4cb052-7b5b-4ec8-b1a8-db5294f4ac74)

The previous histogram was created from a NumPy array `ends`, that contains 500 integers. Each integer represents the end point of a random walk. To calculate the chance that this end point is greater than or equal to 60, we can count the number of integers in `ends` that are greater than or equal to 60 and divide that number by 500, the total number of simulations.

Probability of ending at 60 or above: 0.792


