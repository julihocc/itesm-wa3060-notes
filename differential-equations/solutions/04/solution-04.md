### **Solution: Solving Homogeneous Differential Equations**  

A **homogeneous differential equation** is of the form:  
\[
y' = f\left(\frac{y}{x}\right)
\]
which allows the substitution:  
\[
v = \frac{y}{x} \Rightarrow y = vx, \quad \text{so that} \quad y' = v + x \frac{dv}{dx}
\]
This substitution transforms the given equation into a separable form.

---

## **(a) \( y' = \frac{x + y}{x - y} \)**  
### **Step 1: Substituting \( v = \frac{y}{x} \)**
Since \( y = vx \), we differentiate both sides:  
\[
y' = v + x \frac{dv}{dx}
\]
Substituting into the given equation:
\[
v + x \frac{dv}{dx} = \frac{x + vx}{x - vx}
\]
Factor out \( x \) in the fraction:
\[
\frac{x(1 + v)}{x(1 - v)} = \frac{1 + v}{1 - v}
\]
Thus, we obtain:
\[
v + x \frac{dv}{dx} = \frac{1 + v}{1 - v}
\]

### **Step 2: Separating Variables**
Rearrange to solve for \( dv/dx \):
\[
x \frac{dv}{dx} = \frac{1 + v}{1 - v} - v
\]
\[
x \frac{dv}{dx} = \frac{1 + v - v(1 - v)}{1 - v}
\]
\[
x \frac{dv}{dx} = \frac{1 + v - v + v^2}{1 - v} = \frac{1 + v^2}{1 - v}
\]
Rearrange:
\[
\frac{(1 - v)}{1 + v^2} dv = \frac{dx}{x}
\]

### **Step 3: Integrate Both Sides**
Using substitution for the left integral, let \( u = 1 + v^2 \), then \( du = 2v dv \):
\[
\int \frac{(1 - v)}{1 + v^2} dv = \int \frac{dv}{1 + v^2} - \int \frac{v dv}{1 + v^2}
\]
\[
= \tan^{-1}(v) - \frac{1}{2} \ln(1 + v^2)
\]
For the right integral:
\[
\int \frac{dx}{x} = \ln |x|
\]

### **Step 4: Solve for \( y \)**
\[
\tan^{-1}(y/x) - \frac{1}{2} \ln(1 + (y/x)^2) = \ln |x| + C
\]

✅ **Final Answer:**  
\[
\tan^{-1}(y/x) - \frac{1}{2} \ln(1 + (y/x)^2) = \ln |x| + C
\]

---

## **(b) \( y' = \frac{x^2 + y^2}{xy} \)**  
### **Step 1: Substituting \( v = \frac{y}{x} \)**
\[
y = vx, \quad y' = v + x \frac{dv}{dx}
\]
Substituting into the given equation:
\[
v + x \frac{dv}{dx} = \frac{x^2 + v^2 x^2}{x v x}
\]
\[
= \frac{x^2(1 + v^2)}{x^2 v} = \frac{1 + v^2}{v}
\]
Thus, we obtain:
\[
v + x \frac{dv}{dx} = \frac{1 + v^2}{v}
\]

### **Step 2: Separating Variables**
\[
x \frac{dv}{dx} = \frac{1 + v^2}{v} - v
\]
\[
x \frac{dv}{dx} = \frac{1 + v^2 - v^2}{v} = \frac{1}{v}
\]
\[
v dv = \frac{dx}{x}
\]

### **Step 3: Integrate Both Sides**
\[
\int v dv = \int \frac{dx}{x}
\]
\[
\frac{v^2}{2} = \ln |x| + C
\]

### **Step 4: Solve for \( y \)**
\[
\frac{(y/x)^2}{2} = \ln |x| + C
\]
\[
y^2 = 2x^2 (\ln |x| + C)
\]

✅ **Final Answer:**  
\[
y^2 = 2x^2 (\ln |x| + C)
\]

---

### **Final Answers Summary:**
| Equation | Solution |
|-----------|------------|
| \( y' = \frac{x + y}{x - y} \) | \( \tan^{-1}(y/x) - \frac{1}{2} \ln(1 + (y/x)^2) = \ln |x| + C \) |
| \( y' = \frac{x^2 + y^2}{xy} \) | \( y^2 = 2x^2 (\ln |x| + C) \) |

Let me know if you need further clarification! 😊