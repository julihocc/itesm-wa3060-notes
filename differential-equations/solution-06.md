### **Solution: Determining Exactness and Solving the Equations**  

A first-order differential equation of the form  
```math
M(x, y)dx + N(x, y)dy = 0
```
is **exact** if it satisfies the exactness condition:  
```math
\frac{\partial M}{\partial y} = \frac{\partial N}{\partial x}
```
If the equation is exact, there exists a potential function $F(x, y)$ such that:  
```math
\frac{\partial F}{\partial x} = M, \quad \frac{\partial F}{\partial y} = N
```
Solving for $F(x, y)$ gives the implicit solution $F(x, y) = C$.

---

## **(a) $(2xy + y^2)dx + (x^2 + 2xy)dy = 0$**  
### **Step 1: Identify $M(x, y)$ and $N(x, y)$**
```math
M(x, y) = 2xy + y^2, \quad N(x, y) = x^2 + 2xy
```

### **Step 2: Check Exactness Condition**
Compute $\frac{\partial M}{\partial y}$ and $\frac{\partial N}{\partial x}$:

```math
\frac{\partial M}{\partial y} = \frac{\partial}{\partial y} (2xy + y^2) = 2x + 2y
```

```math
\frac{\partial N}{\partial x} = \frac{\partial}{\partial x} (x^2 + 2xy) = 2x + 2y
```

Since $\frac{\partial M}{\partial y} = \frac{\partial N}{\partial x}$, the equation is **exact**.

### **Step 3: Find the Potential Function $F(x, y)$**
We need a function $F(x, y)$ such that:
```math
\frac{\partial F}{\partial x} = M = 2xy + y^2
```
Integrate with respect to $x$:
```math
F(x, y) = \int (2xy + y^2) dx = x^2y + y^2x + g(y)
```
where $g(y)$ is an arbitrary function of $y$.

Now, differentiate $F(x, y)$ with respect to $y$ and set it equal to $N(x, y)$:
```math
\frac{\partial}{\partial y} (x^2y + y^2x + g(y)) = x^2 + 2xy + g'(y)
```

Since $N(x, y) = x^2 + 2xy$, we compare:
```math
x^2 + 2xy + g'(y) = x^2 + 2xy
```

Thus, $g'(y) = 0$ so $g(y) = C$.

### **Step 4: Final Solution**
```math
x^2y + y^2x = C
```

✅ **Final Answer:**
```math
x^2y + y^2x = C
```

---

## **(b) $(y + 3x^2y^2)dx + (x + 2x^3y)dy = 0$**  
### **Step 1: Identify $M(x, y)$ and $N(x, y)$**
```math
M(x, y) = y + 3x^2y^2, \quad N(x, y) = x + 2x^3y
```

### **Step 2: Check Exactness Condition**
Compute $\frac{\partial M}{\partial y}$ and $\frac{\partial N}{\partial x}$:

```math
\frac{\partial M}{\partial y} = \frac{\partial}{\partial y} (y + 3x^2y^2) = 1 + 6x^2y
```

```math
\frac{\partial N}{\partial x} = \frac{\partial}{\partial x} (x + 2x^3y) = 1 + 6x^2y
```

Since $\frac{\partial M}{\partial y} = \frac{\partial N}{\partial x}$, the equation is **exact**.

### **Step 3: Find the Potential Function $F(x, y)$**
We need a function $F(x, y)$ such that:
```math
\frac{\partial F}{\partial x} = M = y + 3x^2y^2
```
Integrate with respect to $x$:
```math
F(x, y) = \int (y + 3x^2y^2) dx = xy + x^3y^2 + g(y)
```
where $g(y)$ is an arbitrary function of $y$.

Now, differentiate $F(x, y)$ with respect to $y$ and set it equal to $N(x, y)$:
```math
\frac{\partial}{\partial y} (xy + x^3y^2 + g(y)) = x + 2x^3y + g'(y)
```

Since $N(x, y) = x + 2x^3y$, we compare:
```math
x + 2x^3y + g'(y) = x + 2x^3y
```

Thus, $g'(y) = 0$ so $g(y) = C$.

### **Step 4: Final Solution**
```math
xy + x^3y^2 = C
```

✅ **Final Answer:**
```math
xy + x^3y^2 = C
```

---

### **Final Answers Summary:**
| Equation | Solution |
|-----------|------------|
| $(2xy + y^2)dx + (x^2 + 2xy)dy = 0$ | $x^2y + y^2x = C$ |
| $(y + 3x^2y^2)dx + (x + 2x^3y)dy = 0$ | $xy + x^3y^2 = C$ |
