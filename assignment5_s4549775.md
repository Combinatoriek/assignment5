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

	$x^2 - 8x + 16$ for $x = r^2$

	$\begin{aligned}
		x_{1, 2} &= -\frac{-8}{2} \pm \sqrt{(\frac{-8}{2})^2 - 16}\\
		x_{1, 2} &= 4 \pm \sqrt{4^2 - 16}\\
		x_{1, 2} &= 4
	\end{aligned}$

	$x_1 = 4$ for $x_1 = r^2$, so $r_1 = 2, r_2 = -2$

	$x_2 = 4$ for $x_2 = r^2$, so $r_3 = 2, r_4 = -2$

Now we rewrite $F(n)$:

$F(n) = b_0 * s^n, b_0 = 1, s = -2$

$s$ is a root of the recurrence relation with multiplicity 2, therefore the particular solution is of the form $n^2 p_0 (-2)^n$.

## b
We rewrite $F(n)$:

$F(n) = b_2 n^2 s^n, b_2 = 1, s = 4$

$s$ is not a root the the recurrence relation (see (a)), therefore the particular solution is of the form $(p_2 n^2 + p_1 n + p_0) 4^n$.

## c
We rewrite $F(n)$:

$F(n) = b_4 n^4 s^n, b_4 = 1, s = 2$

$s$ is a root of the recurrence relation with multiplicity 2 (see (a)), therefore the particular solution is of the form $n^2 b_4 n^4 2^n = b_4 n^6 2^n$.

# 11
## a
1. The default form is

	$a_n = -5a_{n - 1} -6a_{n - 2} + 42 * 4^n$

2. The characteristic equation is

	$\begin{aligned}
		r^2 - c_1 r - c_2 &= 0\\
		r^2 + 5 r + 6 &= 0
	\end{aligned}$

3. Find the roots $r_i$.

	$\begin{aligned}
		r_{1, 2} &= -\frac{5}{2} \pm \sqrt{(\frac{5}{2})^2 - 6}\\
		r_{1, 2} &= -2.5 \pm \sqrt{\frac{25}{4} - 6}\\
		r_{1, 2} &= -2.5 \pm \sqrt{\frac{1}{4}}\\
		r_{1, 2} &= -2.5 \pm \frac{1}{2}
	\end{aligned}$

	$r_1 = -2, r_2 = -3$

4. The general solution is

	$\begin{aligned}
		a_n^{(h)} &= \alpha_1 r_1^n + \alpha_2 r_2^n\\
		&= \alpha_1 (-2)^n + \alpha_2 (-3)^n
	\end{aligned}$

5. Find a particular solution

	We can use *Theorem 6*: $F(n) = b_0 s^n, b_0 = 42, s = 4$

	$\begin{aligned}
		a_n &= p_0 4^n\\
		a_{n - 1} &= p_0 4^{n - 1}\\
		a_{n - 2} &= p_0 4^{n - 2}
	\end{aligned}$

	$\begin{aligned}
		p_0 4^n &= -5p_0 4^{n - 1} -6p_0 4^{n - 2} + 42 * 4^n\\
		p_0 4^2 &= -5p_0 4 -6p_0 + 42 * 4^2\\
		16 p_0 &= -20p_0 -6p_0 + 672\\
		42 p_0 &= 672\\
		p_0 &= 16
	\end{aligned}$

	$a_n^{(p)} = 16 * 4^n$

6. Add $a_n^{(h)}$ and $a_n^{(p)}$

$\begin{aligned}
	a_n &= \alpha_1 (-2)^n + \alpha_2 (-3)^n + 16 * 4^n\\
	&= \alpha_1 (-2)^n + \alpha_2 (-3)^n + 4^{n + 2}
\end{aligned}$

## b
$\begin{aligned}
	56 &= \alpha_1 (-2)^1 + \alpha_2 (-3)^1 + 4^3\\
	-8 &= -2 \alpha_1 + -3 \alpha_2
\end{aligned}$

$\begin{aligned}
	278 &= \alpha_1 (-2)^2 + \alpha_2 (-3)^2 + 4^4\\
	22 &= 4 \alpha_1 + 9 \alpha_2
\end{aligned}$

$\alpha_1 = 1, \alpha_2 = 2$

$a_n = 1 (-2)^n + 2 (-3)^n + 4^{n + 2}$

# 12
1. The default form is

	$a_n = 4a_{n - 1} -3a_{n - 2} + 2^n$ + n + 3

2. The characteristic equation is

	$\begin{aligned}
		r^2 - c_1 r - c_2 &= 0\\
		r^2 - 4 r + 3 &= 0
	\end{aligned}$

3. Find the roots $r_i$.

	$\begin{aligned}
		r_{1, 2} &= -\frac{-4}{2} \pm \sqrt{(\frac{-4}{2})^2 - 3}\\
		&= 2 \pm \sqrt{\frac{16}{4} - 3}\\
		&= 2 \pm 1
	\end{aligned}$

	$r_1 = 1, r_2 = 3$

4. The general solution is

	$\begin{aligned}
		a_n^{(h)} &= \alpha_1 r_1^n + \alpha_2 r_2^n\\
		&= \alpha_1 + \alpha_2 3^n
	\end{aligned}$

# 13
## a
$s_1 = 1$, because 0 is even. If we do not use a blue marble the requirement is fulfilled, and we only have 1 marble in total. We can select a yellow or red marble, and put it into 1 bag.

$s_2 = 2$. We can use 2 marbles selected from the yellow and red ones, and put them in 2 different bags. Using 2 blue marbles we cannot match or surpass this, because we need to put them into the same bag.

## b
## c
