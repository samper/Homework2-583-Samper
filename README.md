
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
