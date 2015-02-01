---
categories: data
author: Arnob Alam
---

Sometimes having more data can actually cloud the relationships between
between variables.  Let's look at a model of something experiencing geometric
growth (like your bank account, hopefully) random shocks.

Let's start with a model where there is no randomness. You deposit
$$Y(0)$$ in your bank acount at time $$t=0$$ which pays interest $$r$$.
You want to find out how much money you will have at time $$t=1$$:

$$
Y(1) = Y(0) + Y(0)*r = Y(0)(1+r)
$$

You don't take out the money at $$t=1$$ so it continues to accrue interest.
How much money will you have at time $$t=2$$?

$$
Y(2) = Y(1) + Y(1)*r = Y(1)(1+r) \\
\because Y(1) = Y(0) + Y(0)*r = Y(0)(1+r) \\
\therefore Y(2) = Y(0)(1+r)(1+r) = Y(0)(1+r)^2
\ldots \\
$$

In general, at some time t, the amount of money you will have is:

$$
Y(t) = Y(0)(1+r)^t \\
$$