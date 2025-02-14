
# Answer Key

---

## Question 1

a) **Sample Space:**  
For a fair coin toss, $\Omega=\{H, T\}$.

b) **Disjoint Events:**  
Events $A$ (“Head”) and $B$ (“Tail”) are disjoint because they cannot occur simultaneously in a single coin toss.

---

## Question 2

We know:
$$
P(A\cup B)=P(A)+P(B)-P(A\cap B).
$$
So,  
a)  
$$
P(A\cap B)=0.4+0.5-0.7=0.2.
$$

b)  
$$
P(A^c\cap B^c)=1-P(A\cup B)=1-0.7=0.3.
$$

---

## Question 3

a) **Sample Space:**  
$$
\{HH,\ HT,\ TH,\ TT\}.
$$

b) **Event $C$:** “Exactly one head” corresponds to $\{HT,\ TH\}$.  
Thus,  
$$
P(C)=\frac{2}{4}=0.5.
$$

c) **Independence Check:**  
- Let $F$ = “first toss is a head” with outcomes $\{HH, HT\}$, so $P(F)=\frac{2}{4}=0.5$.  
- Intersection $F\cap C=\{HT\}$ with $P(F\cap C)=\frac{1}{4}=0.25$.  
- Since $P(F)P(C)=0.5\times0.5=0.25$ and $P(F\cap C)=0.25$, the events are independent.

---

## Question 4

$X\sim \text{Binomial}(10,0.3)$.

a)  
$$
P(X=3)=\binom{10}{3}(0.3)^3(0.7)^7.
$$
Calculation:  
$\binom{10}{3}=120$,  
$(0.3)^3=0.027$,  
$(0.7)^7\approx0.08235$.  
Thus,  
$$
P(X=3)\approx 120\times 0.027\times 0.08235\approx 0.2668.
$$

b)  
$$
E[X]=np=10\times0.3=3,
$$
$$
\mathrm{Var}(X)=np(1-p)=10\times0.3\times0.7=2.1.
$$

---

## Question 5

$Y\sim \text{Uniform}(2,8)$.

a) **PDF:**  
$$
f_Y(y)=\frac{1}{8-2}=\frac{1}{6},\quad 2\le y\le 8.
$$

b)  
$$
P(3\le Y\le 5)=\int_3^5\frac{1}{6}\,dy=\frac{5-3}{6}=\frac{2}{6}=\frac{1}{3}\approx0.3333.
$$

---

## Question 6

$X\sim N(100,16^2)$.

a) **Z-scores:**

For $X=90$:  
$$
z=\frac{90-100}{16}=-\frac{10}{16}=-0.625.
$$

For $X=110$:  
$$
z=\frac{110-100}{16}=\frac{10}{16}=0.625.
$$

b)  
$$
P(90\le X\le110)=P(-0.625\le Z\le0.625).
$$
Using standard normal tables:
- $P(Z\le0.625)\approx0.7340$,
- $P(Z\le-0.625)\approx0.2660$.  
Thus,  
$$
P(90\le X\le110)\approx0.7340-0.2660=0.4680.
$$

---

## Question 7

Population parameters: $\mu=10$ and $\sigma^2=9$.

a) **Sampling Distribution:**  
For a sample of size $n=36$, the sampling distribution of $\bar{X}$ is:
$$
\bar{X}\sim N\Bigl(10,\frac{9}{36}\Bigr)=N(10,0.25).
$$

b)  
Standard error: $\sigma_{\bar{X}}=\sqrt{0.25}=0.5$.  
Compute:
$$
P(\bar{X}\le 11)=P\Bigl(\frac{\bar{X}-10}{0.5}\le \frac{11-10}{0.5}\Bigr)=P(Z\le2).
$$
From the Z-table, $P(Z\le2)\approx0.9772$.

---

## Question 8

For $n=25$, $\bar{X}=50$, $s=4$, degrees of freedom $=24$.  
Using the t-distribution, the 95% confidence interval is:
$$
\bar{X}\pm t_{\alpha/2,\,n-1}\cdot\frac{s}{\sqrt{n}}.
$$
From t-tables, $t_{0.025,24}\approx2.064$.  
Margin of error:
$$
2.064\times\frac{4}{5}=2.064\times0.8\approx1.6512.
$$
Thus, the 95% CI for $\mu$ is approximately:
$$
(50-1.65,\;50+1.65)=(48.35,\;51.65).
$$

---

## Question 9

A **parameter** is a numerical characteristic of a population (e.g., the true average income of all residents in a city, say $\mu=60,\!000$ dollars). A **statistic** is a numerical measure computed from a sample (e.g., the sample mean income calculated from 200 randomly selected residents). The statistic is used to estimate the parameter.

---

## Question 10

a) **Distribution Identification:**  
The number of products meeting the standard follows a Binomial distribution:  
$$
X\sim \text{Binomial}(n=100,\,p=0.7).
$$

b)  
$$
P(X=75)=\binom{100}{75}(0.7)^{75}(0.3)^{25}.
$$
(Leave the answer in this exact form or compute numerically if required.)

c) **Normal Approximation:**  
For $X\sim \text{Binomial}(100,0.7)$:
- Mean: $\mu=np=70$,
- Variance: $\sigma^2=np(1-p)=21$,
- Standard deviation: $\sigma\approx\sqrt{21}\approx4.583$.

For $P(X\ge68)$, use continuity correction:
$$
P(X\ge68)\approx P\bigl(Y\ge67.5\bigr),
$$
where $Y$ is $N(70,4.583^2)$.  
Compute the z-score:
$$
z=\frac{67.5-70}{4.583}\approx\frac{-2.5}{4.583}\approx-0.546.
$$
Then,
$$
P(Y\ge67.5)=1-P(Z\le -0.546)=1-0.292\approx0.708.
$$
Thus, the approximate probability is about 70.8%.
