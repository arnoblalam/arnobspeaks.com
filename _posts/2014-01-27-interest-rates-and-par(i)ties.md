---
categories: international-finance class-notes
---

# Covered interest rate parity

Covered interest parity refers to the condition that the interest rates and forwards prices move in such a way that any gains due to nominal interest rate differences between two countries is wiped out by the premium on the forward premium.  Formally:

$$
\begin{align*}
f &\equiv \frac{F - S}{S} &= \frac{F}{S} - 1 \\
(1 + i)S &\equiv (1 + i^*)F
\end{align*}
$$

where:

$$S$$ is the spot exchange rate  
$$F$$ is the forward exchange rate  
$$f$$ is the forward premium  
$$i$$ is the domestic interest rate  
$$i^*$$ is the foreign interest rate

The second line is the covered interest rate parity condition.

Manipulating some variables, we obtain:

$$
\begin{align*}
\frac{F}{S} &= \frac{1 + i}{1 + i^*} \\
f &= \frac{F}{S} - 1 \\
&= \frac{i-i^*}{i^*+1} \approx i - i^* \\
\therefore i &\approx i^* + f
\end{align*}
$$

# Uncovered interest rate parity

The uncovered interest rate parity condition states that the differences in nominal interest rates between two countries is explained by the expected change in exchange rates:

$$
i \equiv i^* + \Delta S^e
$$


# How well does it hold up?

Covered intereste parity holds up quite well.  This is likely because traders set ptices on forwards contracts to make the covered interest rate parity condition come true.  Uncovered interest rate parity conditions do not hold up as well (although what the future expected interest rate is, is hard to measure).