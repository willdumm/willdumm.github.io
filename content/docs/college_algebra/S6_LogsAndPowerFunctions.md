---
title: "§6 Logarithms and Power Functions"
math: true
---

How do you solve an equation like $5 = 3^x$ for $x$? You use logarithms.

---

#### Definition (Log Functions)

If $b^L = a$, then we say that $L = \log_b(a)$, or read out loud, "$L$ is the log, base $b$, of $a$."

Also, the "natural log" is defined to be the base $e$ logarithm, and written
$\ln(x) = \log_e(x)$.

If the base $b$ of the log is not specified, then you should assume the base is
$10$. That is, $\log(x) = \log_{10}(x)$.

---

So we can for example solve an equation like $5 = 3^x$ using the base 3 log:
$\log_3(5) = x$. Some calculators can compute this directly, but usually we
only can compute natural logs and base 10 logs. Luckily, there are some useful
rules to help convert between logarithms:

---

#### Log Rules:

Rule | Example
-|-
$\log(a) + \log(b) = \log(ab)$ | $\log(5) + \log(2) = \log(10)$
$\log(a) - \log(b) = \log\left(\frac{a}{b}\right)$ | $\log(6) - \log(2) = \log(3)$
$n\log(a) = \log(a^n)$ | $\log(5^x) = x\cdot \log(5)$
$\log_b(a) = \frac{\log_c(a)}{\log_c(b)}$, for any $c$. **"change of base "** | $\log(5) = \frac{\ln(5)}{\ln(10)}$
$b^{\log_b(x)} = x$ | $10^{\log(t + 3)} = t+3$
$\log_b(b^x) = x$ | $\log(e^{3t}) = 3t$
$\log_b(b) = 1$ | $\log(10) = 1$ 
$\log_b(1) = 0$ | $\ln(1) = 0$

---

Now, we can rewrite $\log_3(5) = \frac{\ln(5)}{\ln(3)}$, which is something
that we can put in any calculator.


---

A **logarithmic function** is any function of the form $f(t) = a + \log_b(t)$,
with domain  $(0, \infty)$.


## Power Functions:

---

#### Definition

A function $f$ is a power function if it can be written in the form $f(t)
= a(t)^b$, for $a$ a positive constant, and $b$ any constant.

---

You will encounter examples of relationships that can be modeled with power
functions in homework.

You will frequently be asked to write an equation for a power function that
passes through two points. For example,

> Find the equation for a power function that passes through the points $(2, 5)$ and $(5, 25)$.

* First, we identify that since our function is a power function, it will have
    the form $f(t) = a(t)^b$.
* Using the two points given, we can write the equations
 $$\begin{aligned}
 5 &= a(2)^b\\\\
 25&=a(5)^b\end{aligned}$$
* Solving the first equation for  $a$, we have $a = \frac{5}{2^b}$, and we can
    substitute this into the second equation to get
    $$25 = \frac{5}{2^t}(5)^t = 5\left(\frac{5}{2}\right)^b$$
    To solve this for $b$, we divide both sides by $5$ and then take the log of
    both sides:
    $$\begin{aligned}
    5 &= \left(\frac{5}{2}\right)^b\\\\[10pt]
    \log(5) &= \log\left(\left(\frac{5}{2}\right)^b\right)\\\\[10pt]
    \log(5) &= b\log\left(\frac{5}{2}\right)\\\\[10pt]
    b &= \frac{\log(5)}{\log\left(\frac{5}{2}\right)}\end{aligned}$$

* Finally, now that we have an expression for $b$, we can substitute it into
    the earlier expression for $a$ :
    $$a = \frac{5}{2^{\frac{\log(5)}{\log(\frac{5}{2})}}}$$

* Putting both expressions into a calculator, we find that $b=1.76$ and $a=1.48$, so $f(t) = 1.48(t)^{1.76}$.
