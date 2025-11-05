# Average or amortized case analysis 
- with average case analysis i hypotize the input is random so that i can achive an average case which is normally less than the worst case scenario, in this 
#### Hiring problem 
- i want to calculate on avarage how many person i need do change to get the best applicant over a set of n applicants
- expected number of hiring is logn

# Las Vegas and Montecarlo
Answer can be only **yes or no**
### Las Vegas
- is always right
It is considered a **efficient** algorithm when his expected running time is bounded by a **polynomial function of the input size**

### Montecarlo 
- can be wrong :
	- only when it says yes(or no) -> **one-sided**
	- always -> **two-sided**
- we can calculate the expected probability of the wrong answer
It is considered a **efficient** algorithm when his running time of the **worst case** is bounded by a **polynomial function of the input size**

##### Example
### Monte Carlo
![[Pasted image 20251104174250.png]]
The runtime is fixed and is O(k)
### Las Vegas
![[Pasted image 20251104174232.png]]
runtime is upper bounded by O(1) in the best case and arbitrarly large in worst case

