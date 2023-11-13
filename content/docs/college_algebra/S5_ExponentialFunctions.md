---
title: "§5 Exponential Functions"
math: true
---

### Percentage Change

Recall that before talking about linear functions, we discussed average rate of
change of a function.

There's another way to talk about the average change of a function on an
interval, and this is **percentage change**

---

The **percentage change** of a function $f$ on an interval $[a,b]$ is given by
$$ PC_{[a,b]} = \frac{f(b) - f(a)}{f(a)} * 100\%$$

---

For example, the percentage change of $f(t) = t^2 - t + 1$ on the interval $[0,2]$
is 
$$PC_{[0,2]} = \frac{f(2) - f(0)}{f(0)} * 100\% = \frac{3 - 1}{1}*100\%
= 200\%$$

A function that changes by a constant percentage for each 1-unit increase in
its input variable is called an **exponential function**.


Maybe you've heard the story about a king who agreed to give one of his
subjects a single grain of rice, and each day after that for 64 days, to give
twice as many grains of rice as he had the day before. On the first day, the
king would need to give only $1*2$ grains of rice. On the second day, he would
have to give $(1*2)*2 = 1*2^2$ grains of rice, and on the third day, he would
have to give $(1*2^2)*2 = 1*2^3$ grains of rice. On the $t^{th}$ day, the king
would have to give $1*2^t$ grains of rice. Although for the first few days, he
would have to give only a few grains of rice each day, on the 64th day he would
have to give about 636 trillion pounds of rice. Each day, the amount of rice
gifted increases by a factor of 2 (or $200\%$).

This is the sort of relationship that exponential functions model. 

### Equations for Exponential Functions:
There are three common forms for exponential functions. They are all the same
kind of function, and you can use any one of them to find any other one. In
each of these forms, $a$ is a positive constant, which is the initial value of
the function: $f(0) = a$.

* $f(t) = ab^t$, where $b$ is a positive constant called the
    **constant growth factor** or just **growth factor**.
* $f(t) = a(1+r)^t$, where $r$ is greater than $-1$, and is called the
    **relative growth rate**.
*  $f(t) = ae^{kt}$, where $e$ is the number (approximately 2.72), and $k$ is a constant called the **continuous growth rate**. We also say that $Q=f(t)$ changes at a rate
    proportional to itself, with constant of proportionality $k$. 

#### Example:
1) Suppose we have an exponential function given by $f(t) = 2(1.8)^t$.

    * Then the constant growth factor of $f$ is $1.8$.
    * By solving $1+r = 1.8$ for $r$, we get $r=0.8$, and we can rewrite $f$ as
        $f(t) = 2(1+0.8)^t$. From this we see that the relative growth rate is $0.8$, or $80\%$.
    * By solving $e^k = 1.8$ for $k$, we get $k=ln(1.8) = 0.59$, so we can rewrite
        $f$ as $f(t) = 2e^{0.59t}$. From this we see that the continuous growth
        rate is $0.59$, or $59\%$.
2) Suppose we are given the following problem:

   > The population of bacteria in a culture is proportional to itself, with
   constant growth rate $1.2$. After 2 hours there are 12 billion bacteria in
   the culture. Write an equation for the number of bacteria after $t$ hours

   * We know this will be an exponential function, and we're given the constant
       growth rate, so we should use the form $f(t) = ae^{kt}$, with $k = 1.2$.
   * We need to find $a$, so we will use the fact that after 2 hours there are
       12 billion bacteria. In other words, $f(2) = 12 = ae^{1.2(2)}$. Then $a
       = \frac{12}{e^{2.4}} = 1.089$, so the population of bacteria in billions
       after $t$ hours is given by $f(t) = 1.089e^{1.2t}$.
3) Suppose we are given the following problem:

    > Find an equation for an exponential function which passes through the
    points $(2,1)$ and $(4,9)$.

    * First, we know we need an exponential function, so let's use the simplest
    one, $f(t) = ab^t$.
    * From the first point given, we know that when we put $2$ into $f$, we get
        an output of $1$, so we have the equation $f(2) = 1 = ab^2$. Similarly
        the other point gives us the equation $f(4) = 9 = ab^4$.
    * Solving the first equation for $a$, we see that $a = \frac{1}{b^2}$.
        Substituting this for $a$ in the second equation, we get
        $$9 = \frac{1}{b^2}b^4 = b^2$$
        so  $b = \sqrt{9} = 3$. ($-3$ could also work, but $b$ needs to be
        positive.)
    * Finally, we can find $a$ using the fact that we already used, $a
        = \frac{1}{b^2} = \frac{1}{9}$.

### Compounded Interest:

There is one final form for the equation of an exponential function, which we
will use when modeling interest which is compounded.

If a quantity of money $a$ is invested at an interest rate $r$, and the
interest is compounded $n$ times per year, then after $t$ years, the value of
the investment is given by
$$f(t) = a\left(1+\frac{r}{n}\right)^{nt}$$

For example, if $12000 is invested at $2\%$ interest, compounded monthly, then
the value of the investment after $t$ years is given by

$$12000\left(1+\frac{0.02}{12}\right)^{12t}$$

## Long-Term Behavior of Exponential Functions:

Exponential functions are all either increasing or decreasing on its entire
domain. This is determined by their growth factor, relative growth factor, or
continuous growth rate.

If an exponential function has... | ... then it is:
---|---
growth factor $b\gt 1$ | increasing
growth factor $b\lt 1$ | decreasing
relative growth rate $r \gt 0$ | increasing
relative growth rate $r\lt 0$ | decreasing
continuous growth rate $k\gt 0$ | increasing
continuous growth rate $k\lt 0$ |  decreasing


These two different kinds of exponential functions look like the following two
examples:

![s5graph1](figures/s5graph1.pdf)

![s5graph2](figures/s5graph2.pdf)

So, as can be seen from the graphs, an increasing exponential function
approaches $\infty$ as  $t$ increases without bound, while a decreasing
exponential function approaches $0$.

If a quantity is modeled by an increasing exponential function, we say it
exhibits **exponential growth**.

If a quantity is modeled by a decreasing exponential function, we say it
exhibits **exponential decay**.
