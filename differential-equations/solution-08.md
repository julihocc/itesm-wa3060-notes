### **Solution: Newton’s Law of Cooling**  

Newton’s Law of Cooling states that the rate of change of the temperature of an object is proportional to the difference between its temperature and the ambient temperature:  
```math
\frac{dT}{dt} = -k (T - T_{\infty})
```
where:  
- $T(t)$ is the temperature at time $t$,  
- $T_{\infty} = 20^\circ C$ is the ambient temperature,  
- $k$ is the cooling constant,  
- $T_0 = 90^\circ C$ is the initial temperature.

---

### **Step 1: Solve the Differential Equation**
This is a separable equation:
```math
\frac{dT}{T - 20} = -k dt
```
Integrating both sides:
```math
\int \frac{dT}{T - 20} = \int -k dt
```
```math
\ln |T - 20| = -kt + C
```
Exponentiate both sides:
```math
T - 20 = e^{-kt + C} = e^C e^{-kt}
```
Define $C' = e^C$ (a new constant):
```math
T - 20 = C' e^{-kt}
```

Since $C'$ represents an initial temperature shift, we use the initial condition $T(0) = 90$:
```math
90 - 20 = C' e^{0}
```
```math
C' = 70
```
Thus, the **cooling equation** is:
```math
T(t) = 20 + 70 e^{-kt}
```

✅ **Final Answer for Cooling Equation:**
```math
T(t) = 20 + 70 e^{-kt}
```

---

### **Step 2: Find $k$ Using Given Data**  
We are given $T(5) = 70$:
```math
70 = 20 + 70 e^{-5k}
```
```math
50 = 70 e^{-5k}
```
Divide by 70:
```math
\frac{50}{70} = e^{-5k}
```
```math
\frac{5}{7} = e^{-5k}
```
Take the natural logarithm:
```math
\ln \frac{5}{7} = -5k
```
```math
k = -\frac{\ln \frac{5}{7}}{5}
```

Approximating $\ln(5/7) \approx -0.3365$:
```math
k \approx \frac{0.3365}{5} = 0.0673
```

---

### **Step 3: Find $T(10)$**
Substituting $t = 10$ into $T(t) = 20 + 70 e^{-0.0673 t}$:
```math
T(10) = 20 + 70 e^{-0.0673(10)}
```
```math
T(10) = 20 + 70 e^{-0.673}
```
Approximating $e^{-0.673} \approx 0.5105$:
```math
T(10) = 20 + 70(0.5105)
```
```math
T(10) = 20 + 35.74
```
```math
T(10) \approx 55.74
```

✅ **Final Answer for Temperature After 10 Minutes:**
```math
T(10) \approx 55.7^\circ C
```

---

### **Final Answers Summary:**
1. **Cooling Equation:**  
   ```math
   T(t) = 20 + 70 e^{-0.0673t}
   ```
2. **Temperature after 10 minutes:**  
   ```math
   T(10) \approx 55.7^\circ C
   ```
