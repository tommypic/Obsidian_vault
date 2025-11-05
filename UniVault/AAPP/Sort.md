# Quicksort(pivot, list)
- complexity of time: $nlog(n)$
- it is a **divide and conqueer algorithm**
- sorts in place
## how it works
- pivot is the first element
- i start with pivot, i put all elements bigger than pivot to the left and smaller to right
- i put the pivot in the middle
- i call the algorithm on the two division
### cost of the algorithm 
- the cost of rearranging the elements is O(n)
- worst case is $O(n^2)$
	- i find that all elements are bigger(or smaller) then the pivot
$$ T(n) = T(0) + T(n-1) + cn$$
- i get a recursion tree that is of heigh n so i need to sum all the cn and i get a $O(n^2)$
- best case i that the pivot each time divide the array in two perfectly divided arrays so i get a time coplexity of $O(nlog(n))$
- almost best case is also $O(nlog(n))$ 


## How fast can we sort
All algorithm we analized are comparison sort algorithm, that are upper bounded by a 
$$O(nlgn)$$ best case of time complexity.
because we always get a comparison tree that is always of heigh of nlogn

# Counting Sort
in this algorithm we don't do any comparison between elements
![[Pasted image 20251104191700.png]]
counting sort can take $O(n+k)$, where k is the max value that we can see in the array, so if k = O(n ) we get the final time complexity to be O(n)
counting sort is not a comparison sort

## Stable sorting
- if a algorithm of sorting is stable it preserve the 


