### **Solution: Solving Separable Differential Equations**  

A **separable equation** is an equation that can be written in the form:  
```math
\frac{dy}{dx} = f(x)g(y)
```
which allows separation of variables:  
```math
\frac{dy}{g(y)} = f(x)dx
```
After separation, we integrate both sides to find the general solution.  

---

### **(a) $\frac{dy}{dx}=xy$**  
#### **Step 1: Separate Variables**  
```math
\frac{dy}{y}=xdx
```
#### **Step 2: Integrate Both Sides**  
```math
\int \frac{dy}{y}=\int xdx
```
```math
\ln |y|=\frac{x^2}{2}+C
```
#### **Step 3: Solve for $y$**  
```math
y=e^{C}e^{x^2/2}
```
Since $e^C$ is an arbitrary constant, we define $C'=e^C$:  
```math
y=C'e^{x^2/2}
```
✅ **Final Answer:**  
```math
y=Ce^{x^2/2}, \quad C \text{ is an arbitrary constant.}
```

---

### **(b) $\frac{dy}{dx}=\frac{x}{y}$**  
#### **Step 1: Separate Variables**  
```math
y \, dy= x \, dx
```
#### **Step 2: Integrate Both Sides**  
```math
\int y \, dy=\int x \, dx
```
```math
\frac{y^2}{2}=\frac{x^2}{2}+C
```
#### **Step 3: Solve for $y$**  
```math
y^2=x^2+2C
```
```math
y=\pm \sqrt{x^2+2C}
```
✅ **Final Answer:**  
```math
y=\pm \sqrt{x^2+C}, \quad C \text{ is an arbitrary constant.}
```

---

### **(c) $y'=e^x y$**  
#### **Step 1: Separate Variables**  
```math
\frac{dy}{y}=e^x \, dx
```
#### **Step 2: Integrate Both Sides**  
```math
\int \frac{dy}{y}=\int e^x \, dx
```
```math
\ln |y|=e^x+C
```
#### **Step 3: Solve for $y$**  
```math
y=e^C e^{e^x}
```
Define $C'=e^C$:  
```math
y=C'e^{e^x}
```
✅ **Final Answer:**  
```math
y=Ce^{e^x}, \quad C \text{ is an arbitrary constant.}
```

---

### **(d) $(y^2+1) \, dy=x \, dx$**  
#### **Step 1: Separate Variables**  
```math
\frac{dy}{y^2+1}=x \, dx
```
#### **Step 2: Integrate Both Sides**  
```math
\int \frac{dy}{y^2+1}=\int x \, dx
```
The left integral is a standard form:  
```math
\int \frac{dy}{y^2+1}=\tan^{-1}(y)
```
The right integral is straightforward:  
```math
\int x \, dx=\frac{x^2}{2}+C
```
#### **Step 3: Solve for $y$**  
```math
\tan^{-1}(y)=\frac{x^2}{2}+C
```
```math
y=\tan \left( \frac{x^2}{2}+C \right)
```
✅ **Final Answer:**  
```math
y=\tan \left( \frac{x^2}{2}+C \right), \quad C \text{ is an arbitrary constant.}
```

---

### **Final Answers Summary:**
| Equation | Solution |
|-----------|------------|
| $\frac{dy}{dx}=xy$ | $y=Ce^{x^2/2}$ |
| $\frac{dy}{dx}=\frac{x}{y}$ | $y=\pm \sqrt{x^2+C}$ |
| $y'=e^x y$ | $y=Ce^{e^x}$ |
| $(y^2+1) \, dy=x \, dx$ | $y=\tan \left( \frac{x^2}{2}+C \right)$ |
