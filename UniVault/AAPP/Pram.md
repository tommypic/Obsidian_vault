Is a machine model **M** with theese components:
-  rams M1,M2 ... M, which are all the rams of 
- input cells X(1), X(2), ...
- output cells Y(1), ...
- shared memory cells A(1),...
## Assumtions
- infinite registers
- infinte memory cells
- each memory cell can contain infinite long int
- no **communication overhead**
## Types of Write and Read conflict
- **ER** exclusive read
- **CR** concurrent read
- **EW** exclusive write
- **CW** concurrent write
	- pritority, there is a priority of writes
	- common, wirte is all same values
	- random, choose randomly who writes
## Definitions
![[Pasted image 20251104154132.png]]

## MVM algorithm 
Matrix vector multiply algorithm: each multiplication of row with vector is handled on each processor
- perfect efficiency for all p 
- speedup = p
- because i have that $T_1 = T^*$  
## SUM 
I use logarithmic, i sum elements two by two and add them 
- i gen a log(n) tree
![[Pasted image 20251104160320.png]]
![[Pasted image 20251104160418.png]]
## Matrix Multiply
![[Pasted image 20251104160441.png]]

PROCESSOR 𝑃𝑖,𝑗,𝑙 COMPUTES 𝐴𝑖,𝑙𝐵𝑙,𝑗
so i need p = $n^3$

## Amdahl's Law and Gustafson law 
- amdahl say that the amount of parallelizable code is fixed i always have a fixed amount of serial code so if the serial code is 1/10 of the total the maximum speedup is 10 since the serial remains
- he support the **hard scaling**
- **workload is fixed **

![[Pasted image 20251104161404.png]]
![[Pasted image 20251104161430.png]]


- For gustawsono the datawill be more carefully and fully analyzed if the computer power increase , he support the **weak scaling**
- weak scaling support the face that if the **number of processor increase it increase also the workload**
![[Pasted image 20251104162313.png]]
![[Pasted image 20251104162340.png]]


