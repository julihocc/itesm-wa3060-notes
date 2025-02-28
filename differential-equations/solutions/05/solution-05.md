### **Solution: Solving First-Order Linear Differential Equations Using the Integrating Factor Method**  

A first-order linear differential equation is of the form:  
\[
y' + P(x)y = Q(x)
\]
The solution is found using the **integrating factor** \( \mu(x) \), given by:  
\[
\mu(x) = e^{\int P(x)dx}
\]
Multiplying the entire equation by \( \mu(x) \) allows us to write the left-hand side as a derivative, which can then be integrated.

---

### **(a) \( y' + 2y = e^{-x} \)**  
#### **Step 1: Identify \( P(x) \) and \( Q(x) \)**
\[
P(x) = 2, \quad Q(x) = e^{-x}
\]

#### **Step 2: Compute the Integrating Factor**
\[
\mu(x) = e^{\int 2dx} = e^{2x}
\]

#### **Step 3: Multiply the Equation by \( \mu(x) \)**
\[
e^{2x} y' + 2e^{2x}y = e^{2x} e^{-x}
\]
\[
\frac{d}{dx} \left( e^{2x} y \right) = e^x
\]

#### **Step 4: Integrate Both Sides**
\[
\int d(e^{2x} y) = \int e^x dx
\]
\[
e^{2x} y = e^x + C
\]

#### **Step 5: Solve for \( y \)**
\[
y = e^{-2x} (e^x + C)
\]
\[
y = e^{-x} + C e^{-2x}
\]

✅ **Final Answer:**
\[
y = e^{-x} + C e^{-2x}
\]

---

### **(b) \( xy' + y = x^2 \)**  
#### **Step 1: Rewrite in Standard Form**
Divide by \( x \) to get:
\[
y' + \frac{y}{x} = x
\]
Thus, \( P(x) = \frac{1}{x} \) and \( Q(x) = x \).

#### **Step 2: Compute the Integrating Factor**
\[
\mu(x) = e^{\int \frac{dx}{x}} = e^{\ln x} = x
\]

#### **Step 3: Multiply the Equation by \( \mu(x) \)**
\[
x y' + y = x^2
\]
\[
\frac{d}{dx} (x y) = x^2
\]

#### **Step 4: Integrate Both Sides**
\[
\int d(xy) = \int x^2 dx
\]
\[
xy = \frac{x^3}{3} + C
\]

#### **Step 5: Solve for \( y \)**
\[
y = \frac{x^2}{3} + \frac{C}{x}
\]

✅ **Final Answer:**
\[
y = \frac{x^2}{3} + \frac{C}{x}
\]

---

### **(c) \( y' + \frac{y}{x} = \sin x \)**  
#### **Step 1: Identify \( P(x) \) and \( Q(x) \)**
\[
P(x) = \frac{1}{x}, \quad Q(x) = \sin x
\]

#### **Step 2: Compute the Integrating Factor**
\[
\mu(x) = e^{\int \frac{dx}{x}} = e^{\ln x} = x
\]

#### **Step 3: Multiply the Equation by \( \mu(x) \)**
\[
x y' + y = x \sin x
\]
\[
\frac{d}{dx} (x y) = x \sin x
\]

#### **Step 4: Integrate Both Sides**
\[
\int d(xy) = \int x \sin x dx
\]

Using integration by parts for \( \int x \sin x dx \):  
Let \( u = x \), \( dv = \sin x dx \), then  
\( du = dx \), \( v = -\cos x \).  

\[
\int x \sin x dx = -x \cos x + \int \cos x dx
\]
\[
= -x \cos x + \sin x
\]

Thus, integrating both sides:
\[
xy = -x \cos x + \sin x + C
\]

#### **Step 5: Solve for \( y \)**
\[
y = -\cos x + \frac{\sin x}{x} + \frac{C}{x}
\]

✅ **Final Answer:**
\[
y = -\cos x + \frac{\sin x}{x} + \frac{C}{x}
\]

---

### **Final Answers Summary:**
| Equation | Solution |
|-----------|------------|
| \( y' + 2y = e^{-x} \) | \( y = e^{-x} + C e^{-2x} \) |
| \( xy' + y = x^2 \) | \( y = \frac{x^2}{3} + \frac{C}{x} \) |
| \( y' + \frac{y}{x} = \sin x \) | \( y = -\cos x + \frac{\sin x}{x} + \frac{C}{x} \) |
