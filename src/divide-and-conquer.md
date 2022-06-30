# Divide and Conquer

## Basic Log Rules

1. \\(log_b{(b)} = 1\\)
2. \\(log_b{(mn)} = log_b{m} + log_b{n}\\)
3. \\(log_b{(\frac{m}{n})} = log_b{m} - log_b{n}\\)
4. \\(log_b{(m^n)} = n \cdot log_b{m}\\)
5. \\(log_b{(b^m)} = m\\)

## Substitution Method

The big idea is to *guess* at the solution, then solve by induction.
* The trick that got me is that you *start* with the induction hypothesis.

## Summation Method

Basically the tree method - add up the costs of the nodes.
* Produce a geometric sequence

## Master Theorem

Given a recurrence relation \\(T(n) = aT(\tfrac{n}{b}) + f(n)\\), where \\(a \geq 1\\) and \\(b > 1\\) are two positive constants, the asymptotic bound of \\(T(n)\\) can be obtained in the following cases:

1. If \\(f(n) = O(n^{\log_b{(a - \epsilon)}})\\) for some constant \\(\epsilon > 0\\), then \\(T(n) = \Theta(n^{log_b{(a)}})\\)