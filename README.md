# Simulated annealing
## Solution, which solves the salesmen problem for 30 top-populated cities of Russia.

### Goal 
The mail goal was to find the optimal path using the Simulated Annealing algorithm for 
30 most populated cities of Russian Federation. Secondary goal was to track the speed 
of convergence for different values of cooling rate and compare the results. 

![30 top populated cities in Russia](/images/cities_empty.png)

### Distance function
As it was mentioned in the task, we are dealing with geodesic coordinates. 
To correctly evaluate the distance between the cities on the globe the [haversine formula](https://en.wikipedia.org/wiki/Haversine_formula) was used.

### Experiment conditions
The initial temperature was set to 10000. 
For a cooling rate the following values were used:
* 0.003
* 0.01
* 0.1

## Results
The following will include the results on an experiments and several 
conclusions based on the observations. On a map the red dot (and red 
title) for the city mean that it is the start city.

### Slow cooling
The best route for slow cooling value 0.003 was **19074.21 km**
![The best route for slow cooling](/images/cities_slow.png)

Slow cooling requires over 3000 iterations
![Convergence for slow cooling](/plots/plot_slow.png)

### Average cooling
The best route for average cooling value 0.01 was **24457.48 km**
![The best route for average cooling](/images/cities_average.png)

Average cooling requires a bit more than 900 iterations
![Convergence for slow cooling](/plots/plot_average.png)

### Fast cooling
The best route for fast cooling value 0.1 was **37499.90 km**
![The best route for fast cooling](/images/cities_fast.png)

Fast cooling requires nearly 90 iterations
![Convergence for slow cooling](/plots/plot_fast.png)

### Observations
As we see, as the cooling rate descreases, the precision of approximation of the global optimum is increasing.  
