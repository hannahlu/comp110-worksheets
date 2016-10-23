>>> Worksheet C: Computational Complexity

A)	The algorithm performs a check for duplications in a list, with n being the length of the list. If a duplication is found then the procedure returns True, if no duplications are found in list then the procedure returns False.

B)	The worst case running time is quadratic O(N)² because the program has a for loop nested within the first for loop and therefore, the amount of iterations needed increases by the square of the input size. The program would have been linear had the second list not been nested in the first, and adding a new loop would increase the number of iterations proportionally. However, with this quadratic algorithm, if n = 6, for every iteration of the first loop, the inner loop will perform 6 loops: with each increase of the input, the loops on the second iteration will be n².

C)	The algorithm is still correct; the procedure now only runs through j as far as i – 1. The procedure will only check a value against values that came before it in the list. This stops the procedure from checking a value against the same value multiple times and stops a value being checked against itself.

D)	The algorithm will run approximately twice as fast because the procedure no longer needs to perform as many iterations. The procedure no longer checks the same two values against each other more than once and no longer checks a value against itself. Overall this roughly halves the number of iterations.

E)	The time complexity is now

F)	The time complexity of Python’s built-in [1] SORT () function is O (n log n).

G)	The procedure’s computational complexity is O (n log n); the procedure uses the SORT () function with the time complexity of O (n log n). For large input values the addition of a for loop with time complexity O(n) would not make a significant difference, and therefore the procedure overall can still be said to have a time complexity of O (n log n).

H)	The second procedure is likely to be faster with a larger input; this is because each value only needs to be checked with the one before it. O (n log n) will run faster with a larger input than O (n)² as it has better scalability.

I)	A programmer may choose to use the slower procedure rather than the faster because they have a very small input size and therefore scalability is not of concern. 

Reference List:

[1] B. Rocky (2015, June. 15). “Time Complexity”. Python Wiki. [Online]. Available: https://wiki.python.org/moin/TimeComplexity [Accessed: Oct. 23. 2016]

