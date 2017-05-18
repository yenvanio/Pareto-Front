## Pre-existing Algorithms that are being used for Non-dominant Sorting

```
<b>Algorithm:</b> Kung's Algorithm

Sort the population in descending order of importance in the first objective function and rename the population as P of size N.
Front(P):
if |P| ← 1 then 
	return P else
T ← Front(P(1) – P(|P/2|)) and B ← Front(P(|P|/2+1) – P(P)) 

If the ith non-dominated solution B is not dominated by any non-dominated solution of T,create a merged set M ← T*U*i. 
	return M

Algorithm: Ding’s Algorithm
Input: X
Output: The non-dominated set – X0 of X
(R0 stores the non-dominate set of rank set R) 
Using quick-sort method to create indices I1, I2...IM and rank ← R;

R0 = I1(1)0s, I2(1)0s…IM(1)0s and eliminate the duplicate ones
for (i ← 1; i*N; increment i by 1) 
 	stop ← N; //Set initial termination position N; 
for (i ← 2; i*stop; increment i by 1) //Search at the ith entry of index Ij;
if (Ij(i)0s not checked) then 
	Compare it with the non-dominated ones among ij(1)0s; ij(2)0s … ij(i ¡ 1)0s and set it checked
if (Ij(i)0s is not dominated by any of them) then 
	put Ij(i)0s in R0
i0 ← max of its ranks (or components); 
stop ← minStop, i0g; //Update termination position

```

<b>Algorithm:</b> Jun Du Algorithm (Sorting based Algorithm) 

<ol>
<li> The population of solutions is sorted according to
the descending order to every objective functions.
Thereafter, several solutions sequences could be presented
and each of them corresponds to one objective. Every
solution could be scored according to the position it takes,
higher score it gains. Then, each solution could get various scores corresponding to various objectives. Take the scores
summation of every solution, and sort it to get one new
solution summation sequence. The new summation
sequence could be used for finding non dominated set by
deleting all the dominated solution inside. </li>
<li>The bottom of the summation sequence is used as
the start of the compared solution, while the top of the
summation sequence is used as the start of the comparing
one. Once the compared solution is observed by any one
anterior to it, it is deleted. When the compared solution
becomes the top one of the sequence, the dominated set is
drawn out.</li>
</ol>
