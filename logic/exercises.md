### **Exercises: Logic**  

#### **1. Propositional and First-Order Logic**  
1. Determine whether the following statements are **tautologies**, **contradictions**, or **contingent**:  
   a) $P \lor \neg P$  
   b) $(P \lor Q) \land (\neg P \lor \neg Q)$  
   c) $(P \rightarrow Q) \lor (Q \rightarrow P)$  
   d) $(P \land Q) \rightarrow P$  

2. Construct the **truth table** for the following expressions:  
   a) $(P \lor Q) \rightarrow R$  
   b) $(P \land Q) \lor (\neg P \land \neg Q)$  
   c) $\neg (P \lor Q) \equiv \neg P \land \neg Q$  

3. Translate the following statements into **propositional logic**:  
   a) "If it is raining, then the ground is wet."  
   b) "Either Alice or Bob will win the competition, but not both."  
   c) "If the alarm is not working, then either there is a power failure or the battery is dead."  

---

#### **2. Formalization of Arguments**  
4. Determine whether the following arguments are **valid** using **truth tables** or **logical inference rules**:  

   a) **Premises:**  
      - $P \rightarrow Q$  
      - $Q \rightarrow R$  
      - $P$  
      **Conclusion:** $R$  

   b) **Premises:**  
      - $P \lor Q$  
      - $\neg P$  
      **Conclusion:** $Q$  

   c) **Premises:**  
      - $(P \rightarrow Q) \land (Q \rightarrow R)$  
      - $\neg R$  
      **Conclusion:** $\neg P$  

5. Use **natural deduction** to prove the following statements:  
   a) $P \lor (Q \land R) \vdash (P \lor Q) \land (P \lor R)$  
   b) $(P \rightarrow Q) \land (R \rightarrow S), P \lor R \vdash Q \lor S$  

---

#### **3. Applications in Mathematics and Computation**  
6. **Set Theory Application:** Let $U = \{1,2,3,4,5,6,7,8,9\}$, $A = \{2,4,6,8\}$, and $B = \{1,2,3,4\}$. Compute:  
   a) $A \cup B$  
   b) $A \cap B$  
   c) $A^c$ (the complement of $A$ in $U$)  
   d) $(A \cup B)^c$  

7. **Boolean Algebra and Circuits:** Simplify the following Boolean expressions using **Boolean algebra laws**:  
   a) $(A \lor B) \land (\neg A \lor B)$  
   b) $(A \land B) \lor (\neg A \land B)$  
   c) $A \lor (A \land B)$  

8. **Logic Programming (Prolog):** Given the facts:  
   ```prolog
   parent(alice, bob).
   parent(bob, charlie).
   parent(charlie, david).
   ```  
   a) Write a **recursive rule** for the "ancestor" relation.  
   b) Query whether **Alice is an ancestor of David** using your rule.
