---
title: "§0 Prerequisites and Helpful Info"
math: true
---


### How to Round Properly
Sometimes there's confusion about how to properly round an answer. Suppose you
compute an answer $5.79782$, and are asked to round it to the nearest whole
number. Well, the two nearest whole numbers are $5$ and $6$, but since the
first decimal place of our answer is occupied by a $7$, our number $5.79782$ is
more than halfway between $5$ and $6$, so we should round to $6$.

Similarly, if we were asked to round $3.746$ to one decimal place, we would
need to decide if $3.746$ is closer to $3.7$ or $3.8$. In this case, since the
next digit is less than $5$, our number is less than halfway between $3.7$ and
$3.8$, so the correct choice is $3.7$.


Finally, suppose we are asked to round $3.74501$ to two decimal places (or "the
nearest hundredth"). We would need to decide which of all the numbers with two
decimals is closest to $3.74$. The closest two numbers
with two decimals are $3.74$ and $3.75$, but notice that $3.74501$ is slightly
more than halfway between $3.74$ and $3.75$, so the correct answer is $3.75$.

There is a convention that if you are asked to round something like $3.5$ to
the nearest whole number, then even though it is exactly halfway between the
two candidates, $3$ and $4$, you should round up and choose $4$. This is
basically a personal preference and depends on what the number means, and you won't encounter this situation in this
class.

### Some Useful Exponent Rules

You need to know the following facts for this class about exponents:

Fact | Why? | Example
-|-|-
$x^{ab} = (x^a)^b = (x^b)^a$ |$x^6 = xxxxxx = (xx)(xx)(xx) = (xx)^3 = (x^2)^3$  | $5^{2t} = (5^2)^t = 25^t$
 $x^a\cdot x^b = x^{a+b}$ | $x^3\cdot x^2 = (xxx)(xx) = xxxxx = x^5$ | $x^3\cdot x^2 = x^5$
 $\sqrt[n]{x} = x^{\frac{1}{n}}$ | That's just how it is (by the first fact). |  $\sqrt{x} = x^\frac{1}{2}$

 Also, you should know that if you have an equation like $5^t = 4$, you can get
 $t$ out of the exponent by taking the log of both sides: $t\log(5) = \log(4)$.
 Also, if you have an equation like $\log(t) = 3$, then you can take $10$ to
 the power of both sides: $10^{\log(t)} = 10^3$. The left side of this equation
 is just $t$.

### How to Use Interval Notation

Interval notation allows us to compactly describe sets of real numbers.
The thing to remember, is that `(` and `[` mean different things:

* $[a, b]$ means "all numbers between $a$ and $b$, including $a$ and $b$."
* $(a, b)$ means "all numbers between $a$ and $b$, not including $a$ and $b$."
* $[a, b)$ means "all numbers between $a$ and $b$, including $a$ but not
including $b$."
* $(a,b]$ means "all numbers between $a$ and $b$, not including $a$ but including
$b$."

We can use **unions** to combine multiple intervals. For example, $(a,b)\cup
(c,d)$ means "all the numbers between, but not including $a$ and $b$, **and**
all the numbers between, but not including, $c$ and $d$."

Also, if we want to use intervals to express the sentence "all the numbers
greater than 7" we could write $(7,\infty)$, the interval from $7$ to infinity.

If we want to use intervals to express the sentence "all numbers other than 1",
we could write  $(-\infty, 1)\cup (1,\infty)$. The first interval includes all
numbers less than $1$, not including $1$, and the second interval includes all
numbers greater than $1$, not including $1$.


### How to Solve a System of Equations

Suppose you find yourself with two equations, like

$$
\begin{aligned}
  1&=b+2a \\\\
  -17&=a-3b
\end{aligned}
$$

... and you want to find out what the values of $a$ and $b$ must be. (This may
seem like an unlikely situation to find yourself in, but I promise it will
happen a lot!)

Here's how you go about this (**the steps are the same no matter what  the
equations are!**)

1) First, **solve one of the equations for either $a$ or $b$.** In this case, I'll
solve the first equation for $b$, and get $b=1-2a$.

2) Now, **substitute the expression you found for $a$ or $b$ into the other**
equation (the one you didn't use already). In this example, I need to
substitute $1-2a$ wherever I see a $b$ in the equation $-17 = a-3b$.
When I do this, I get:
$$-17 = a - 3(1-2a)$$

3) Now **solve this equation for the unknown**, which in this case is $a$. This is possible since $a$ is the only
unknown variable:
$$\begin{aligned}
-17 &= a - 3(1-2a)\\\\
-17 &= a - 3 +6a\\\\
-17 &= 3 +7a\\\\
-14 &= 7a\\\\
a &= \frac{-14}{7} = -2
\end{aligned}$$

4) Now that we know the value of one of the variables, **we use the equation we
found in step 1 to find the value of the other variable**. In this case, I know
that $a = -2$, and  from step 1 I know that $b = 1-2a$. Substituting $-2$ for
$a$, I get $b = 1-2(-2) = 1 - (-4) = 5$, so $b = 5$.


To practice, try solving a few more systems of equations using the same steps:

* $2a + 2b = 3$ and $-1 + 4b = a$
* $3a-4=2+6b$ and $7b = a-2$.
* There will be plenty more opportunities to practice soon.
