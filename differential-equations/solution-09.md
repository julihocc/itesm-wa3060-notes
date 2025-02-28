### **Solution: Falling Object with Air Resistance**  

The motion of the falling object is governed by the differential equation:  
\[
m \frac{dv}{dt} = mg - kv
\]
where:  
- \( m = 5 \) kg (mass of the object),  
- \( g = 9.8 \) m/s² (acceleration due to gravity),  
- \( k = 2 \) Ns/m (air resistance constant),  
- \( v(0) = 0 \) (initial velocity since the object is dropped from rest).  

---

### **Step 1: Rewrite the Equation in Standard Form**  
Dividing both sides by \( m \):
\[
\frac{dv}{dt} + \frac{k}{m} v = g
\]
Substituting \( k = 2 \) and \( m = 5 \):
\[
\frac{dv}{dt} + \frac{2}{5} v = 9.8
\]
This is a **first-order linear differential equation** of the form:
\[
\frac{dv}{dt} + P v = Q
\]
where \( P = \frac{2}{5} \) and \( Q = 9.8 \).

---

### **Step 2: Solve Using the Integrating Factor Method**  
The integrating factor is:
\[
\mu(t) = e^{\int \frac{2}{5} dt} = e^{\frac{2}{5}t}
\]

Multiplying both sides of the equation by \( \mu(t) \):
\[
e^{\frac{2}{5}t} \frac{dv}{dt} + \frac{2}{5} e^{\frac{2}{5}t} v = 9.8 e^{\frac{2}{5}t}
\]
Rewriting the left-hand side as a derivative:
\[
\frac{d}{dt} \left( e^{\frac{2}{5}t} v \right) = 9.8 e^{\frac{2}{5}t}
\]

### **Step 3: Integrate Both Sides**  
\[
\int d\left(e^{\frac{2}{5}t} v \right) = \int 9.8 e^{\frac{2}{5}t} dt
\]

The right-hand integral is:
\[
\int 9.8 e^{\frac{2}{5}t} dt = 9.8 \cdot \frac{5}{2} e^{\frac{2}{5}t} = 24.5 e^{\frac{2}{5}t}
\]

Thus, we obtain:
\[
e^{\frac{2}{5}t} v = 24.5 e^{\frac{2}{5}t} + C
\]

### **Step 4: Solve for \( v(t) \)**
Dividing by \( e^{\frac{2}{5}t} \):
\[
v = 24.5 + C e^{-\frac{2}{5}t}
\]

Using the initial condition \( v(0) = 0 \):
\[
0 = 24.5 + C e^0
\]
\[
C = -24.5
\]

Thus, the velocity function is:
\[
v(t) = 24.5 (1 - e^{-\frac{2}{5}t})
\]

✅ **Final Answer for Velocity Function:**
\[
v(t) = 24.5 (1 - e^{-\frac{2}{5}t})
\]

---

### **Step 5: Find the Terminal Velocity**  
The **terminal velocity** is the velocity as \( t \to \infty \), which means \( e^{-\frac{2}{5}t} \to 0 \):

\[
v_{\text{terminal}} = 24.5 (1 - 0) = 24.5 \text{ m/s}
\]

✅ **Final Answer for Terminal Velocity:**
\[
v_{\text{terminal}} = 24.5 \text{ m/s}
\]

---

### **Final Answers Summary:**
1. **Velocity function:**  
   \[
   v(t) = 24.5 (1 - e^{-\frac{2}{5}t})
   \]
2. **Terminal velocity:**  
   \[
   v_{\text{terminal}} = 24.5 \text{ m/s}
   \]
