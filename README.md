# Pareto-Front
Research to decrease the time complexity to find the Pareto Frontier

## Pseudocode

```

Array of X Points
Array of Y Points

Sort the Arrays (Ascending or Descending)

Create a List of Points (Java Class, pairs of x and y)
Put corresponding X, Y points in the list

Create a Pareto Frontier
Initialize it with the first point from the list

Loop through the list
.  If Max Y Value
.  .  If current pair in list >= previous pair in Pareto Frontier (Finding Higher Y Values)
.  .   Add pair to Pareto Frontier
.  Else
.    If current pair in list <= previous pair in Pareto Frontier (Finding Lower Y Values)
.      Add pair to Pareto Frontier
Return Pair.

```


Project Collaborators: 
  - Sai Pedamallu
    - https://github.com/jrsai 
    
