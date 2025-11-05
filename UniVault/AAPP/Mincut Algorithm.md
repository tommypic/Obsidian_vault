Mincut Algorithm aims to find the minimum cut between a connected set of vertices.
![[Pasted image 20251104180332.png]]
-Krages approach is based on a randomized approach
-  i start on a multigraph
- i try to contract edges![[Pasted image 20251104181749.png]]
When i contract vertices i mantain the minimum possible number of cut
We pick a **random** edge uniformly and we merge the two vertices at its end-points.
if we repeat the algorithm multiple times the probability of success grows
 

the krage algorithm run takes $O(n^2)$
with an error probability that is $1/poly(n)$

### Faster version by krager and stein
- the key idea comes because it's very unlikley that i contract a minimum an edge in the first part of the algorithm, the probability grows in the end.
- you run the original algorithm on down to a less number of vertices
- you recurse on this graph


with a $O(log^2(n))$ of run of the algorithm i have a probability of succes that is $> 1- 1/poly(n)$

 