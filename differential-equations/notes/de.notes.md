# **Lecture Notes: Differential Equations**  

## **1. Introduction to Differential Equations**  
Differential equations are equations that relate a function to its derivatives. They are fundamental in the mathematical modeling of physical, biological, and economic phenomena, among others.  

### **Classification of Differential Equations**  
1. **Ordinary Differential Equations (ODEs):** involve a function of a single independent variable and its derivatives.  
2. **Partial Differential Equations (PDEs):** contain partial derivatives of a function with multiple independent variables.  

### **Order and Linearity**  
- **Order:** defined by the highest derivative present in the equation.  
- **Linear vs. Nonlinear:** An equation is linear if the function and its derivatives appear in a linear manner (without products or nonlinear functions of them).  

---

## **2. First-Order Ordinary Differential Equations**  
These are equations of the form:  
```math
F(x, y, y') = 0
```
or, in explicit form,  
```math
y' = f(x, y)
```

### **Types of First-Order Equations**  
1. **Separable Equations:** can be rewritten as  
   ```math
   g(y) dy = f(x) dx
   ```  
   and solved by direct integration.  
   
2. **Homogeneous Equations:** of the form  
   ```math
   y' = f(y/x)
   ```  
   where the substitution \( v = y/x \) is used.  

3. **First-Order Linear Equations:**  
   ```math
   y' + P(x)y = Q(x)
   ```  
   which are solved using an integrating factor.  

4. **Exact Equations:** satisfy  
   ```math
   M(x, y)dx + N(x, y)dy = 0
   ```
   and the exactness condition  
   ```math
   \frac{\partial M}{\partial y} = \frac{\partial N}{\partial x}
   ```  

---

## **3. Solution Methods and Applications**  
### **Solution Methods**  
1. **Direct integration** (for separable equations).  
2. **Using integrating factors** (for linear equations).  
3. **Applying appropriate variable substitutions** (for homogeneous or reducible equations).  
4. **Checking exactness conditions and finding potential functions** (for exact equations).  

### **Common Applications**  
- **Exponential Growth and Decay:**  
  ```math
  \frac{dy}{dt} = ky
  ```
  with solution \( y(t) = y_0 e^{kt} \).  
- **Newton's Law of Cooling:**  
  ```math
  \frac{dT}{dt} = -k(T - T_{\infty})
  ```
  models the temperature change of a body.  
- **Falling Bodies with Air Resistance:**  
  ```math
  m \frac{dv}{dt} = mg - kv
  ```
  describes the velocity of a falling object.  

This topic lays the foundation for higher-order equations and partial differential equations.