## 1. Probability & Set Theory

**Exercise:**  
Roll a fair six-sided die ($\Omega = \{1,2,3,4,5,6\}$). Find $P(\text{roll} < 4)$.

**Solution:**  

- Outcomes less than 4 are: $\{1,2,3\}$.  
- Total outcomes: 6.  
- Thus,
  $$
  P(\text{roll} < 4) = \frac{3}{6} = \frac{1}{2} = 0.5.
  $$

---

## 2. Operations with Events

**Exercise:**  
If $P(A)=0.4$, $P(B)=0.3$, and $P(A\cap B)=0.1$, find:  

1. $P(A^c)$  
2. $P(A\cup B)$  
3. $P((A\cup B)^c)$

**Solution:**  

1. $P(A^c)=1-P(A)=1-0.4=0.6.$  
2. Using the inclusion-exclusion principle,  
   $$
   P(A\cup B)=P(A)+P(B)-P(A\cap B)=0.4+0.3-0.1=0.6.
   $$
3. $P((A\cup B)^c)=1-P(A\cup B)=1-0.6=0.4.$

---

## 3. Conditional Probability & Independence

**Exercise:**  
Two fair coin tosses: Show that “First toss = Heads” and “Second toss = Heads” are independent.

**Solution:**  

- Let $A$ = “First toss = Heads” and $B$ = “Second toss = Heads”.  
- For a fair coin, $P(A)=\frac{1}{2}$ and $P(B)=\frac{1}{2}$.  
- Since the tosses are independent, the joint probability is  
  $$
  P(A\cap B)=\frac{1}{2}\times\frac{1}{2}=\frac{1}{4}.
  $$
- Also, $P(A)P(B)=\frac{1}{2}\times\frac{1}{2}=\frac{1}{4}$.  
- Since $P(A\cap B)=P(A)P(B)$, the events are independent.

---

## 5. Discrete vs. Continuous RV Examples

**Exercise:**  
A fair coin is tossed 5 times. Let $X$ be the number of heads. Find $P(X=2)$ and $E[X]$.

**Solution:**  

- $X$ follows a Binomial distribution with $n=5$ and $p=0.5$.  
- The probability mass function is:
  $$
  P(X=k)=\binom{5}{k}(0.5)^k(0.5)^{5-k}=\binom{5}{k}(0.5)^5.
  $$
- For $k=2$:
  $$
  P(X=2)=\binom{5}{2}(0.5)^5=\frac{10}{32}=\frac{5}{16}\approx0.3125.
  $$
- The expected value for a Binomial distribution is:
  $$
  E[X]=np=5\times0.5=2.5.
  $$

---

## 6. Normal Distribution & Applications

**Exercise:**  
If $X\sim N(100,16)$, find $P(90\le X\le110)$ using Z-scores or tables.

**Solution:**  

- Mean $\mu=100$ and variance $\sigma^2=16$ so $\sigma=4$.  
- For $X=90$:
  $$
  z=\frac{90-100}{4}=-\frac{10}{4}=-2.5.
  $$
- For $X=110$:
  $$
  z=\frac{110-100}{4}=\frac{10}{4}=2.5.
  $$
- Now,  
  $$
  P(90\le X\le110)=P(-2.5\le Z\le 2.5).
  $$
- Using the standard normal table,  
  $$
  P(Z\le2.5)\approx0.9938\quad\text{and}\quad P(Z\le-2.5)\approx0.0062.
  $$
- Therefore,  
  $$
  P(-2.5\le Z\le2.5)=0.9938-0.0062=0.9876.
  $$

---

## 7. Basic Statistical Inference

**Exercise:**  
You sample 100 people’s heights. Which is the parameter, and which is the statistic?

**Solution:**  

- The **parameter** is a numerical characteristic of the entire population (e.g., the true mean height $\mu$ or true standard deviation $\sigma$).  
- The **statistic** is a numerical summary computed from the sample (e.g., the sample mean $\bar{X}$ or sample standard deviation $s$).  
- Thus, in this case, $\mu$ is the parameter and $\bar{X}$ is the statistic.

---

## 8. Point Estimation & Confidence Intervals

**Exercise:**  
A sample of size $n=25$ from a normal population has $\bar{X}=50$ and $s=4$. Construct a 95% confidence interval for $\mu$.

**Solution:**  

- Since the population is normal and the sample size is small, use the t-distribution with $n-1=24$ degrees of freedom.  
- The 95% confidence interval is given by:
  $$
  \bar{X}\pm t_{\alpha/2,\,n-1}\cdot\frac{s}{\sqrt{n}}.
  $$
- From the t-table, for 24 d.o.f. at the 95% confidence level, $t_{0.025,24}\approx2.064$.  
- Compute the margin of error:
  $$
  \text{Margin of Error} = 2.064\times\frac{4}{\sqrt{25}}=2.064\times\frac{4}{5}=2.064\times0.8\approx1.6512.
  $$
- Thus, the 95% confidence interval for $\mu$ is:
  $$
  50\pm1.65,
  $$
  which is approximately:
  $$
  (48.35,\;51.65).
  $$
