---
categories: data
author: Arnob Alam
---

Sometimes having more data can actually cloud the relationships between variables.  Let's look at a model of something experiencing geometric growth (like the economy, hopefully) with random shocks.

Start with a model where there is no randomness. Assume output (GDP) is a function of the growth rate $$r$$, with an initial starting GDP of $$Y(0)$$.

What will the level of GDP be at time $$t=1$$?

$$
Y(1) = Y(0) + Y(0)*r = Y(0)(1+r)
$$

What will the GDP be at time $$t=2$$?

$$
Y(2) = Y(1) + Y(1)*r = Y(1)(1+r) \\
\because Y(1) = Y(0) + Y(0)*r = Y(0)(1+r) \\
\therefore Y(2) = Y(0)(1+r)(1+r) = Y(0)(1+r)^2
\ldots \\
$$

In general, at some time $$t$$, the GDP will be:

$$
Y(t) = Y(0)(1+r)^t \\
$$

Let's add a bit of randomness to the model. Instead of being able to add a 
specific amount every year, you sometimes have to take out money (for medical 
expenses, for example), or deposit extra money (performance bonus). Let's say
at any