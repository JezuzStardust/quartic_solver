# Quartic Solver
An exact and fast quartic solver for Python
Also includes a quadratic (numerically stable) solver and a simpler cubic solver. 

The quartic solver is a direct implementation of the algorithm developed in
Alberto Giacomo Orellana and Cristiano De Michele. 2020. A
lgorithm 1010: Boosting Efficiency in Solving Quartic Equations with No Compromise in Accuracy. 
ACM Trans. Math. Softw. 46, 2, Article 20 (June 2020), 28 pages. https://doi.org/10.1145/3386241

Feel free to use this as you wish, no guarantees.

Usage:
```
import solvers
solvers.solve_quartic(1e23, 1.00, -7.23, 2)
solvers.solve_cubic(1.0, -3.0, 2.5, 2.1)
solvers.solve_quadratic(23.2, 20)
```
Note: 
`solve_quartic(a,b,c,d)` solves the equation $x^4 + a x^3 + b x^2 + c x + d = 0$. 
`solve_cubic(a, b, c, d)` solves the equation $d x^3 + c x^2 + b x + a = 0$ (note the order and that it is possible to set the coefficient in front of the cubic term. 
`solve_quadratic(a,b)` solves the equation $x^2 + a x + b = 0$. 

I will make the cubic solver more like the others later on. 
