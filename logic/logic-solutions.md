## **1. Propositional and First-Order Logic**  

### **1. Classifying Statements (Tautology, Contradiction, or Contingent)**  

a) $P \lor \neg P$  

- This is a **tautology** because it is always true, regardless of the truth value of $P$. (Law of the excluded middle)  

b) $(P \lor Q) \land (\neg P \lor \neg Q)$  

- This is a **contingent** statement because its truth value depends on the values of $P$ and $Q$.  
- For example, if $P = \text{true}$ and $Q = \text{true}$, the expression evaluates to **false**, but for $P = \text{true}, Q = \text{false}$, it evaluates to **true**.  

c) $(P \rightarrow Q) \lor (Q \rightarrow P)$  

- This is a **tautology** (principle of connexity).  
- Using a truth table, it is always **true** for any values of $P$ and $Q$.  

d) $(P \land Q) \rightarrow P$  

- This is a **tautology**, since if $P \land Q$ is true, then $P$ must be true.  

---

### **2. Truth Tables**  

#### (a) $(P \lor Q) \rightarrow R$  

| $P$ | $Q$ | $R$ | $P \lor Q$ | $(P \lor Q) \rightarrow R$ |
|:---:|:---:|:---:|:---:|:---:|
| T | T | T | T | T |
| T | T | F | T | F |
| T | F | T | T | T |
| T | F | F | T | F |
| F | T | T | T | T |
| F | T | F | T | F |
| F | F | T | F | T |
| F | F | F | F | T |

- The expression is not a tautology, since it is false in some cases.  

---

### **3. Translating to Propositional Logic**  

a) "If it is raining, then the ground is wet."  

- Let $R$ be "It is raining" and $W$ be "The ground is wet".  
- $R \rightarrow W$.  

b) "Either Alice or Bob will win the competition, but not both."  

- Let $A$ be "Alice wins" and $B$ be "Bob wins".  
- $(A \lor B) \land \neg (A \land B)$.  

c) "If the alarm is not working, then either there is a power failure or the battery is dead."  

- Let $A$ be "The alarm is working", $P$ be "There is a power failure", and $B$ be "The battery is dead".  
- $\neg A \rightarrow (P \lor B)$.  

---

## **2. Formalization of Arguments**  

### **4. Checking Argument Validity**  

a) **Premises:**  

- $P \rightarrow Q$  
- $Q \rightarrow R$  
- $P$  
   **Conclusion:** $R$  

- By **Modus Ponens**, from $P \rightarrow Q$ and $P$, we infer $Q$.  
- By **Modus Ponens** again, from $Q \rightarrow R$ and $Q$, we infer $R$.  
- **Valid argument.**  

b) **Premises:**  

- $P \lor Q$  
- $\neg P$  
   **Conclusion:** $Q$  

- By **Disjunctive Syllogism**, if $P \lor Q$ is true and $P$ is false, then $Q$ must be true.  
- **Valid argument.**  

c) **Premises:**  

- $(P \rightarrow Q) \land (Q \rightarrow R)$  
- $\neg R$  
   **Conclusion:** $\neg P$  

- Using **Contraposition**, $Q \rightarrow R$ is equivalent to $\neg R \rightarrow \neg Q$.  
- Since $\neg R$ is given, we conclude $\neg Q$.  
- By **Contraposition** again, $P \rightarrow Q$ implies $\neg Q \rightarrow \neg P$.  
- Since $\neg Q$ is true, $\neg P$ follows.  
- **Valid argument.**  

---

### **5. Natural Deduction Proofs**  

#### a) $P \lor (Q \land R) \vdash (P \lor Q) \land (P \lor R)$  

1. Assume $P \lor (Q \land R)$.  
2. Case 1: If $P$, then both $P \lor Q$ and $P \lor R$ hold.  
3. Case 2: If $Q \land R$, then $P \lor Q$ (since $Q$ is true) and $P \lor R$ (since $R$ is true).  
4. In both cases, $(P \lor Q) \land (P \lor R)$ follows.  

#### b) $(P \rightarrow Q) \land (R \rightarrow S), P \lor R \vdash Q \lor S$  

1. From $(P \rightarrow Q) \land (R \rightarrow S)$, we know both implications hold.  
2. If $P$, then $Q$ follows.  
3. If $R$, then $S$ follows.  
4. Since either $P$ or $R$ is true, then either $Q$ or $S$ must be true.  

---

## **3. Applications in Mathematics and Computation**  

### **6. Set Theory**  

Given $U = \{1,2,3,4,5,6,7,8,9\}$, $A = \{2,4,6,8\}$, $B = \{1,2,3,4\}$:  

a) $A \cup B = \{1,2,3,4,6,8\}$.  
b) $A \cap B = \{2,4\}$.  
c) $A^c = \{1,3,5,7,9\}$.  
d) $(A \cup B)^c = \{5,7,9\}$.  

---

### **7. Boolean Algebra**  

a) $(A \lor B) \land (\neg A \lor B)$  

- Using **distribution**:  
- $(A \land \neg A) \lor (A \land B) \lor (B \land \neg A) \lor (B \land B)$  
- Since $A \land \neg A = 0$ and $B \land B = B$:  
- Result: $(A \land B) \lor B = B$.  

b) $(A \land B) \lor (\neg A \land B)$  

- Factor out $B$:  
- $B \land (A \lor \neg A)$.  
- Since $A \lor \neg A = 1$:  
- Result: $B$.  

c) $A \lor (A \land B)$  

- Using **Absorption**: $A \lor (A \land B) = A$.  

---

### **8. Logic Programming (Prolog)**  

a) Recursive rule:  

```prolog
ancestor(X, Y) :- parent(X, Y).
ancestor(X, Y) :- parent(X, Z), ancestor(Z, Y).
```

b) Query:  

```prolog
?- ancestor(alice, david).
```

Result: **true**.
