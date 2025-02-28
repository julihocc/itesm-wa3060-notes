### **Solution: Exponential Growth & Decay Problem**  

The rate of growth is proportional to the population, which means the population $P(t)$ satisfies the **exponential growth equation**:  
```math
\frac{dP}{dt} = kP
```
where $k$ is the proportionality constant.

---

### **Step 1: Solve the Differential Equation**
This is a separable equation:
```math
\frac{dP}{P} = k dt
```
Integrating both sides:
```math
\int \frac{dP}{P} = \int k dt
```
```math
\ln |P| = kt + C
```
Exponentiate both sides:
```math
P = e^{kt + C} = e^C e^{kt}
```
Define $C' = e^C$ (a new constant):
```math
P(t) = C'e^{kt}
```

Since $C'$ represents the initial population, we write:
```math
P(t) = P_0 e^{kt}
```

---

### **Step 2: Find $k$ Using Initial Conditions**  
We are given:  
- $P(0) = 500$, so  
  ```math
  500 = P_0 e^{k(0)}
  ```
  ```math
  P_0 = 500
  ```
  Thus, the equation simplifies to:
  ```math
  P(t) = 500e^{kt}
  ```

- After 2 hours, $P(2) = 2000$:
  ```math
  2000 = 500e^{2k}
  ```
  Divide by 500:
  ```math
  4 = e^{2k}
  ```
  Take the natural logarithm:
  ```math
  \ln 4 = 2k
  ```
  ```math
  k = \frac{\ln 4}{2} = \frac{\ln 2^2}{2} = \frac{2\ln 2}{2} = \ln 2
  ```
  So $k = \ln 2$.

Thus, the **population function** is:
```math
P(t) = 500 e^{(\ln 2) t}
```

Since $e^{\ln 2} = 2$, we can rewrite it as:
```math
P(t) = 500 \cdot 2^t
```

✅ **Final Answer for $P(t)$:**  
```math
P(t) = 500 \cdot 2^t
```

---

### **Step 3: Find $P(5)$**  
Substituting $t = 5$ into the equation:
```math
P(5) = 500 \cdot 2^5
```
```math
P(5) = 500 \cdot 32
```
```math
P(5) = 16000
```

✅ **Final Answer for $P(5)$:**  
```math
P(5) = 16000 \text{ cells}
```

---

### **Final Answers Summary:**
1. **Population function:** $P(t) = 500 \cdot 2^t$
2. **Population after 5 hours:** $P(5) = 16000$ cells
