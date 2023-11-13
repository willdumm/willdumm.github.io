---
title: "§4 Rational Functions"
math: true
---

---

A **rational function** is a function that can be written in the form
$$f(t) = \frac{p(t)}{q(t)}$$

where $p(t)$ and $q(t)$ are polynomial functions.

The mathematical domain of a rational function includes all values of $t$ for which $q(t)$
is not zero.

---

#### Examples:

* $f(t) = \frac{t+2}{3-t^2 + t}$ is a rational function
* $g(t) = \frac{t^{1.5} + 3}{t}$ is **not** a rational function, because the
    numerator is not a polynomial.
* $h(t) = \frac{1}{t^5}$ is a rational function, because $p(t) = 1$ is
    a (very simple) polynomial.
* $r(t) = \frac{t^2 + 3t - 4}{2t + 6}$ is a rational function, and it is not
    defined when $2t+6 = 0$. That happens when $t = -3$, but nowhere else, so
    the domain of $r$ is $(-\infty, -3)\cup(-3, \infty)$.


#### Example: Write Something as a Rational Function

You may be given an equation that doesn't look like a rational function, and
be asked to rewrite it in the standard form for a rational function. Here's an
example:

> Write the equation $f(t) = \frac{3t}{t-1} - \frac{1-t}{t+3}$ in the standard
rational form $f(t) =\frac{p(t)}{q(t)}$.

Clearly, what we want to do is combine the two fractions which are currently
subtracted. You may recall that to combine fractions which are added or
subtracted, they **must have the same denominator**. Although they don't now,
we can make it so they do.


The trick here is to multiply terms by fancy versions of $1$. We are certainly
allowed to multiply a term in the equation by $1$, so we can also multiply a term by
$\frac{t-1}{t-1}$, for example.

By multiplying one term by $\frac{t-1}{t-1}$ and the other by
$\frac{t+3}{t+3}$, we can make sure both terms have the same denominator:

$$
\begin{aligned}
f(t) &= \frac{3t}{t-1}\cdot\frac{t+3}{t+3} - \frac{t-1}{t-1}\cdot\frac{1-t}{t+3}\\\\[10pt]
f(t) &= \frac{3t(t+3)}{(t-1)(t+3)}- \frac{(1-t)(t-1)}{(t-1)(t+3)}\\\\[10pt]
f(t) &= \frac{3t(t+3)-(1-t)(t-1)}{(t-1)(t+3)}
\end{aligned}
$$

Now we have only one fraction, and by distributing terms and combining like
terms we can see that both the numerator and denominator are polynomials, as
required.


#### Example: Concentration
A common reason to think about rational functions is to model
**concentrations** which change.

For example, consider the following problem:

> When filling his pool, Billy throws in .2 gallons of pool chemicals, then starts
> adding pool water. Each gallon of pool water contains 0.001 gallon of pool
> chemicals. Write an equation for the concentration of pool chemicals in the
> pool after $g$ gallons of pool water are added.

Concentration of a substance in a mixture is given by

$$\text{concentration} = \frac{\text{amount of the substance}}{\text{total amount of
mixture}}$$

The amount of pool chemicals initially is 0.2 gallons, and increases by 0.001
gallon for every gallon of pool water added, so the total amount of pool chemicals in
gallons after  $g$ gallons of pool water are added is given by $0.2 + 0.001g$.

The total amount of mixture in the pool is initially 0.2 gallons of pool
chemicals, so after $g$ gallons of pool water are added, the total amount of
mixture in the pool is $0.2 + g$ gallons.

The concentration of pool chemicals in the pool after $g$ gallons of pool water
are added is then

$$ \frac{0.2 + 0.001g}{0.2 + g}$$
and this is an example of a rational function.

## Long-Term Behavior of Rational Functions

---

#### Theorem:

The long-term behavior of a rational function $f(t) = \frac{p(t)}{q(t)}$ is the
same as the long-term behavior of a ratio of the leading terms of $p$ and $q$.

---

This theorem isn't very self-explanatory, so here are some examples:

1) > find the long-term behavior of
   > $$f(t) = \frac{3t^2 + 4t^3 - 1}{2t + 2}$$

    * We know that the long-term behavior of $f$ is the same as the long-term
      behavior of a ratio of the leading terms of its numerator and denominator.

    * The leading term in the numerator is $4t^3$, and the leading term in the
    denominator is $2t$.

    * So, we just need to find the long-term behavior of $\frac{4t^3}{2t}
    = 2t^2$. But this is just a polynomial, with positive leading term, so as
    $t$ gets large it approaches $\infty$.
    * Therefore $f$ approaches $\infty$.

2) > find the long-term behavior of
   > $$g(t) = \frac{3t^2 + 4t^5 - 1}{2t + 2 + 8t^5}$$
   * We know that the long-term behavior of $f$ is the same as the long-term
     behavior of a ratio of the leading terms of its numerator and denominator.

   * The leading term in the numerator is $4t^5$, and the leading term in the
   denominator is $8t^5$.

   * So, we just need to find the long-term behavior of $\frac{4t^5}{8t^5}
   = \frac{1}{2}$. But this is just a constant, so as
   $t$ gets large it approaches $\frac{1}{2}$.
   * Therefore $f$ approaches $\frac{1}{2}$.

2) > find the long-term behavior of
   > $$g(t) = \frac{3t^2 + 4t^5 - 1}{2t + 2 + 8t^6}$$

   * We know that the long-term behavior of $f$ is the same as the long-term
     behavior of a ratio of the leading terms of its numerator and denominator.

   * The leading term in the numerator is $4t^5$, and the leading term in the
   denominator is $8t^6$.

   * So, we just need to find the long-term behavior of $\frac{4t^5}{8t^6}
   = \frac{1}{2t}$. But notice that as $t$ gets large, we're dividing $1$ by a larger and larger number, so as $t$ increases without bound, $\frac{1}{2t}$ gets closer and closer to $0$.
   * Therefore $f$ approaches $0$.

#### Note:
The last example uses some important reasoning. As $t$ gets large, an
expression like
$$\frac{a}{bt^n}$$

 (where $a$ and $b$ are constants and $n$ is a positive exponent)

 approaches $0$ because we're dividing the
 constant $a$ by a larger and larger number $bt^n$.

