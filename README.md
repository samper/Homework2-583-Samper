Instructions
============
Read the section corresponding to the correspondig homework. 
This week: Howework 4

Homework 2
==========

Computing GCD's: The Euclidean algorithm
----------------------------------------

This program computes GCD's using the Euclidean algorithm. In each step
the algorithm reduces the largest number to the residue when divided by 
the smallest one. This produces the GCD in O(log(min{|a|, |b|}) steps. 


Homework 3
==========

Python vs. Cython
-----------------

I did the first three problems and I am not donde with #4 and #5. I was in
a conference last week and did not have much time to code. If permitted I'll 
submit the rest of the homework later this week. 

In problem 1 I improve the GCD algorithm by writing it in cython. 

In problem 2 I wrote the formula for summing the squares of the numbers from 
1 to n^2. I use the well known formula to compute it fast and improve it by using cython. 
I print all the sums up to a 100000 to test how long it takes. 

In problem 3 I did the obvious sieve up to sqrt(n) to determine if n is prime. Then I improve
the algorithm by using cython. I printed the primes up to 100000. To verify the timing. 



Homework 4
==========

Computational number theory
---------------------------
This homework is suported by the program Homework4 in this repository. 


Exercise 1:
-----------
Here we propose the following conjecture: 
Let a,b,c be positive integers such that gcd(a,b,c)=1, the discriminant  \sqrt(b^2 - 4ac) is not rational
and whenever c is even then the parities of a and b are different. 
there are infinitely many primes of the form ax^2 + bx + c. 

All the values that do not satisfy our conditions can be easily discarded, the first one gives us a divisor for all
evaluations, the second one gives a factorization in integers by factoring the polynomial into linear factors and the
third one makes sure that the polynomial does not evaluate to zero in F_2 (the field with two elements). 
To support this I wrote a program in the file Homework 4, that takes three integers a, b, c and computes how many primes, 
up to 10^3, 10^5, 10^7. I picked some generic elements and printed the results. The computation suggests the conjecture 
should be true. 

Exercise 2: 
-----------

0 : 0

1 : 83003

2 : 83108

3 : 1

4 : 83010

5 : 1

6 : 0

7 : 83104

8 : 83152

9 : 0

10 : 0

11 : 83101

12 : 0

13 : 83077

14 : 83022

This is the table I printed for the problem. We could conjecture two things: 

1) There are infintely many primes congruent to a mod 15 if (a,15)=1. 

2) The distribution of the primes is uniform among the residues a that are relatively prime to 15. 

Exercise 3:
-----------
The number you have is 1234567/8901234. To do this I ran a loop to find b computing 372806624339965*b modulo 37+10^15
and making sure both b and the residue mod 37+10^15 are smaller than 10^7. This gives only one possibility for a and b
and we can verify that the decimal expansion starts with 13869616280169693. 

Homework 5
==========
This homework is supported by the sage file Homework 5 in this repository. 
Breaking RSA
------------
Here factor the number 
4654252230393111226989449826741007006486078009450861095070222439898324342353927553909251532232407850265642079868425916328810273416481567992145162141358151
We use the hint that says that the two prime numbers are very close to each other and run an algorithm asking to 
factor using prime factors close to the square root of n. 
We get the numbers: 

68222080226222296181917368518534332259513625527062166102114730123514248558349

68222080226222296181917368518534332259513625527062166102114730123514248558499

That differ only by 150. 

Homework 6
==========
This homework is supported by the file Homework 6 in this repository. 
Diffie-Hellmann key
-------------------
The secret number of this problem is 79067655658429219567805855344438774741
The computations can be found in the first part of the file

RSA encryption:
---------------
The message is 34197073220901184551129292001394589184880483289566520542660754136539424199979218985
for the given e,n. 
