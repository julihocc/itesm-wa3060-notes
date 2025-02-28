### **Solution: Solving Separable Differential Equations**  

A **separable equation** is an equation that can be written in the form:  
\[
\frac{dy}{dx} = f(x)g(y)
\]
which allows separation of variables:  
\[
\frac{dy}{g(y)} = f(x)dx
\]
After separation, we integrate both sides to find the general solution.  

---

### **(a) $ \frac{dy}{dx} = xy $**  
#### **Step 1: Separate Variables**  
\[
\frac{dy}{y} = xdx
\]
#### **Step 2: Integrate Both Sides**  
\[
\int \frac{dy}{y} = \int xdx
\]
\[
\ln |y| = \frac{x^2}{2} + C
\]
#### **Step 3: Solve for $ y $**  
\[
y = e^{C} e^{x^2/2}
\]
Since $ e^C $ is an arbitrary constant, we define $ C' = e^C $:  
\[
y = C'e^{x^2/2}
\]
✅ **Final Answer:**  
\[
y = Ce^{x^2/2}, \quad C \text{ is an arbitrary constant.}
\]

---

### **(b) $ \frac{dy}{dx} = \frac{x}{y} $**  
#### **Step 1: Separate Variables**  
\[
y dy = xdx
\]
#### **Step 2: Integrate Both Sides**  
\[
\int y dy = \int xdx
\]
\[
\frac{y^2}{2} = \frac{x^2}{2} + C
\]
#### **Step 3: Solve for $ y $**  
\[
y^2 = x^2 + 2C
\]
\[
y = \pm \sqrt{x^2 + 2C}
\]
✅ **Final Answer:**  
\[
y = \pm \sqrt{x^2 + C}, \quad C \text{ is an arbitrary constant.}
\]

---

### **(c) $ y' = e^x y $**  
#### **Step 1: Separate Variables**  
\[
\frac{dy}{y} = e^x dx
\]
#### **Step 2: Integrate Both Sides**  
\[
\int \frac{dy}{y} = \int e^x dx
\]
\[
\ln |y| = e^x + C
\]
#### **Step 3: Solve for $ y $**  
\[
y = e^C e^{e^x}
\]
Define $ C' = e^C $:  
\[
y = C'e^{e^x}
\]
✅ **Final Answer:**  
\[
y = Ce^{e^x}, \quad C \text{ is an arbitrary constant.}
\]

---

### **(d) $ (y^2 + 1) dy = x dx $**  
#### **Step 1: Separate Variables**  
\[
\frac{dy}{y^2 + 1} = xdx
\]
#### **Step 2: Integrate Both Sides**  
\[
\int \frac{dy}{y^2 + 1} = \int xdx
\]
The left integral is a standard form:  
\[
\int \frac{dy}{y^2 + 1} = \tan^{-1}(y)
\]
The right integral is straightforward:  
\[
\int xdx = \frac{x^2}{2} + C
\]
#### **Step 3: Solve for $ y $**  
\[
\tan^{-1}(y) = \frac{x^2}{2} + C
\]
\[
y = \tan \left( \frac{x^2}{2} + C \right)
\]
✅ **Final Answer:**  
\[
y = \tan \left( \frac{x^2}{2} + C \right), \quad C \text{ is an arbitrary constant.}
\]

---

### **Final Answers Summary:**
| Equation | Solution |
|-----------|------------|
| $ \frac{dy}{dx} = xy $ | $ y = Ce^{x^2/2} $ |
| $ \frac{dy}{dx} = \frac{x}{y} $ | $ y = \pm \sqrt{x^2 + C} $ |
| $ y' = e^x y $ | $ y = Ce^{e^x} $ |
| $ (y^2 + 1) dy = x dx $ | $ y = \tan \left( \frac{x^2}{2} + C \right) $ |

Let me know if you need further clarification! 😊