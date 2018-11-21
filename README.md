# Simulated annealing
## Solution, which solves the salesmen problem for top-30 cities of Russia.

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
* 0.03
* 0.1

## Results

### Slow cooling
The 
