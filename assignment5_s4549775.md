% Assignment 5\
	Group 4

---
author: Hendrik Werner s4549775
date: \today
fontsize: 12pt
geometry: margin=5em
---

# 8

# 9
## a
$a_n = An + B$

$a_{n - 1} = A(n - 1) + B$

$\begin{aligned}
	An + B &= 2(A(n - 1) + B) + n + 5\\
	&= 2A(n - 1) + 2B + n + 5\\
	&= 2An - 2A + 2B + n + 5\\
	&= 2An + n -2A + 2B + 5
\end{aligned}$

$\begin{aligned}
	2An + n &= An\\
	n(2A + 1) &= An\\
	2A + 1 &= A\\
	A + 1 &= 0\\
	A &= -1
\end{aligned}$

$\begin{aligned}
	-2A + 2B + 5 &= B\\
	-2(-1) + 2B + 5 &= B\\
	2 + 2B + 5 &= B\\
	B + 7 &= 0\\
	B &= - 7
\end{aligned}$

$a_n = -n -7$

## b
1. The default form is

	$a_n = 2a_{n - 1}$

2. The characteristic equation is

	$r - c_1 = 0$

3. Find root $r$.

	$r = c_1 = 2$

4. The general solution is

	$a_n = \alpha_1 2^n$

5. The particular solution is

	$a_n = -n -7$

6. $a_n = \alpha_1 2^n -n -7$

## c
$\begin{aligned}
	\alpha_1 2^0 -0 -7 &= 4\\
	\alpha_1 -7 &= 4\\
	\alpha_1 &= 11
\end{aligned}$

# 10
## a
First we find the roots of the homogeneous part

1. The default form is

	$a_n = 0a_{n - 1} + 8a_{n - 2} + 0a_{n - 3} - 16a_{n - 4}$

2. The characteristic equation is

	$\begin{aligned}
		r^4 - c_1 r^3 - c_2 r^2 - c_3 r - c_4 &= 0\\
		r^4 - 0r^3 - 8r^2 - 0r + 16 &= 0\\
		r^4 - 8r^2 + 16 &= 0
	\end{aligned}$

3. Find the roots $r_i$.

	$x^2 + 8x + 16$ for $x = r^2$

	$\begin{aligned}
		x_{1, 2} &= -\frac{8}{2} \pm \sqrt{(\frac{8}{2})^2 - 16}\\
		x_{1, 2} &= -4 \pm \sqrt{4^2 - 16}\\
		x_{1, 2} &= -4
	\end{aligned}$

	$x_1 = -4$ for $x_1 = r^2$, so $r_1 = 2, r_2 = -2$

	$x_2 = -4$ for $x_2 = r^2$, so $r_3 = 2, r_4 = -2$

Now we rewrite $F(n)$:

$F(n) = b_0 * s^n, b_0 = 1, s = -2$

$s$ is a root of the recurrence relation with multiplicity 2, therefore the particular solution is of the form $p_0 n^2 (-2)^n$.

## b
## c

# 11
## a
## b

# 12

# 13
## a
## b
## c
