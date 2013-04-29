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

I plan to compute the determinant using row echelon form where cython should be considerably faster,
given that it involves doing lots of multiplications. 

For the product of matrices I'll just compute coordinatewise. 

Homework 4
==========

Computational number theory
---------------------------
Exercise 1:
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
