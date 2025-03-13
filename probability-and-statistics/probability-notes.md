# Probability and Statistics Refresher  

### Two-Hour Crash Course

---

# Topics Overview

1. **Probability and Set Theory**  
2. **Operations with Events**  
3. **Conditional Probability and Independence**  
4. **Random Variables and Distributions**  
5. **Discrete vs. Continuous Random Variables**  
6. **Normal Distribution and Its Applications**  
7. **Basic Statistical Inference**  
8. **Point Estimation and Confidence Intervals**

---

# 1. Probability & Set Theory

**Key Points**  

- **Sample space**: $\Omega$, the set of all possible outcomes.  
- **Event**: A subset of $\Omega$.  
- **Axioms**:  
  1. $P(A)\ge0$ for any event $A$.  
  2. $P(\Omega)=1$.  
  3. If $\{A_i\}$ are pairwise disjoint, then
    $$
    P\Bigl(\bigcup_iA_i\Bigr)=\sum_iP(A_i).
    $$

---

**Quick Exercise**  

- Roll a fair six-sided die ($\Omega=\{1,2,3,4,5,6\}$). Find $P(\text{roll}<4)$.

---

# 2. Operations with Events

**Key Points**  

- **Union** ($A\cup B$): either $A$ or $B$ (or both).  
- **Intersection** ($A\cap B$): both $A$ and $B$.  
- **Complement** ($A^c$): not $A$.  
- **De Morgan’s Laws**:  
  - $(A\cup B)^c=A^c\cap B^c$  
  - $(A\cap B)^c=A^c\cup B^c$  
- **Inclusion-Exclusion Principle**:
  $$
  P(A\cup B)=P(A)+P(B)-P(A\cap B).
  $$

---

**Quick Exercise**  

- If $P(A)=0.4$, $P(B)=0.3$, and $P(A\cap B)=0.1$, find $P(A^c)$, $P(A\cup B)$, etc.

---

# 3. Conditional Probability & Independence

**Key Points**  

- **Conditional Probability**:  
  $$
  P(A\mid B)=\frac{P(A\cap B)}{P(B)},\quad P(B)\neq0.
  $$
- **Independence**:  
  Two events $A$ and $B$ are independent if  
  $$
  P(A\cap B)=P(A)P(B).
  $$
- **Chain Rule**:  
  $$
  P(A\cap B\cap C)=P(A)P(B\mid A)P(C\mid A\cap B).
  $$

---

**Quick Exercise**  

- Two fair coin tosses: Show that “First toss=Heads” and “Second toss=Heads” are independent.

---

# 4. Random Variables & Distributions

**Key Points**  

- A **Random Variable (RV)** is a function mapping outcomes in $\Omega$ to real values.  
- **Discrete RV**: Takes values in a countable set.  
- **Continuous RV**: Takes values in an interval of real numbers.  

---

- **PMF** (discrete): $p_X(x)=P(X=x)$.  
- **PDF** (continuous): $f_X(x)$, where
  $$
  P(a\le X\le b)=\int_a^b f_X(x)\,dx.
  $$
- **CDF**: $F_X(x)=P(X\le x)$.  

---

- **Mean**:  
  - Discrete: $E[X]=\sum_x x\,p_X(x)$.  
  - Continuous: $E[X]=\int_{-\infty}^{\infty}x\,f_X(x)\,dx$.  
- **Variance**:
  - $\mathrm{Var}(X)=E[(X-E[X])^2]$
  - Alternatively, $\mathrm{Var}(X)=E[X^2]-(E[X])^2$..

---

# 5. Discrete vs. Continuous RV Examples

**Discrete**  

- **Bernoulli, Binomial, Geometric, Poisson**  
  - Example: **Binomial**$(n,p)$:
    $$
    P(X=k)=\binom{n}{k}p^k(1-p)^{\,n-k}.
    $$

**Continuous**  

- **Uniform, Exponential, Normal**  
  - Example: **Exponential**$(\lambda)$:
    $$
    f_X(x)=\lambda e^{-\lambda x},\quad x\ge0.
    $$

---

**Quick Exercise**  

- A fair coin is tossed 5 times. Let $X$ be the number of heads. Find $P(X=2)$ and $E[X]$.

---

# 6. Normal Distribution & Applications

**Key Points**  

- $X\sim N(\mu,\sigma^2)$:
  $$
  f_X(x)=\frac{1}{\sqrt{2\pi}\,\sigma}\exp\Bigl(-\frac{(x-\mu)^2}{2\sigma^2}\Bigr).
  $$
- **Standard Normal**: $Z\sim N(0,1)$. Any $X\sim N(\mu,\sigma^2)$ can be transformed via
  $$
  Z=\frac{X-\mu}{\sigma}.
  $$
- **68-95-99.7 Rule**: ~68% within $\pm1\sigma$, 95% within $\pm2\sigma$, 99.7% within $\pm3\sigma$.  
- **Central Limit Theorem (CLT)**: For large $n$, the sample mean $\bar{X}$ of i.i.d. RVs is approximately normal.

---

**Quick Exercise**  

- If $X\sim N(100,16)$, find $P(90\le X\le110)$ using Z-scores or tables.

---

# 7. Basic Statistical Inference

**Key Points**  

- **Population vs. Sample**:  
  - Population parameters: $\mu,\sigma$.  
  - Sample statistics: $\bar{X},s$.  
- **Sampling Distribution**: The distribution of a statistic (e.g. $\bar{X}$) over repeated samples.

---

**Quick Exercise**  

- You sample 100 people’s heights. Which is the parameter, and which is the statistic?

---

# 8. Point Estimation & Confidence Intervals

**Key Points**  

- **Point Estimation**:  
  - $\bar{X}$ estimates $\mu$.  
  - $\hat{p}$ estimates the true proportion $p$.  
- **Confidence Intervals**:  
  - For large $n$ with known $\sigma$:
    $$
    \bar{X}\pm z_{\alpha/2}\,\frac{\sigma}{\sqrt{n}}.
    $$
  - If $\sigma$ unknown and $n$ is small, use a **t-distribution** with $n-1$ degrees of freedom.

---

**Quick Exercise**  

- A sample of size $n=25$ from a normal population has $\bar{X}=50$, $s=4$. Construct a 95% CI for $\mu$.

---

# Suggested 2-Hour Agenda

1. **(5 min)** Probability & Set Theory  
2. **(5 min)** Operations with Events  
3. **(10 min)** Conditional Probability & Independence  
4. **(10 min)** Random Variables & Distributions  
5. **(10 min)** Discrete vs. Continuous  
6. **(15 min)** Normal Distribution & Applications  
7. **(15 min)** Basic Statistical Inference  
8. **(20 min)** Estimation & Confidence Intervals  
9. **(30 min)** Extra Practice / Review  

---

# Final Tips

- Focus on **key formulas**: conditional probability, expectation, variance, confidence intervals.  
- Practice with **representative exercises** (binomial, normal, confidence intervals).  
- Use **z-tables / t-tables** for normal or t-distributions.  
- Maintain a simple **checklist**: Did you apply each formula correctly? Interpret results in context?

**Good luck!**
