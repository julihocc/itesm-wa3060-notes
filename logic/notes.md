# **Lecture Notes: Logic**  

## **1. Introduction to Logic**  
Logic is the study of principles of reasoning and argumentation. It provides formal methods for distinguishing valid reasoning from fallacious arguments and is fundamental in mathematics, computer science, and philosophy.  

### **Types of Logic**  
1. **Propositional Logic:** Deals with propositions (statements that are either true or false) and logical connectives such as **AND**, **OR**, and **NOT**.  
2. **First-Order Logic (Predicate Logic):** Extends propositional logic by including quantifiers (**∀, ∃**) and predicates that express relationships between objects.  

---

## **2. Propositional and First-Order Logic**  
### **Propositional Logic**  
A proposition is a declarative statement that can be assigned a truth value (**true** or **false**). Logical connectives allow us to construct compound statements:  

- **Negation ($\neg P$)**: The opposite of $P$.  
- **Conjunction ($P \land Q$)**: True if both $P$ and $Q$ are true.  
- **Disjunction ($P \lor Q$)**: True if at least one of $P$ or $Q$ is true.  
- **Implication ($P \rightarrow Q$)**: True unless $P$ is true and $Q$ is false.  
- **Biconditional ($P \leftrightarrow Q$)**: True if $P$ and $Q$ have the same truth value.  

### **First-Order Logic (FOL)**  
While propositional logic deals with whole statements, **first-order logic** allows us to express statements about objects and their properties using:  
- **Quantifiers**:  
  - **Universal quantifier ($\forall x$)**: "For all $x$, some property holds."  
  - **Existential quantifier ($\exists x$)**: "There exists an $x$ for which a property holds."  
- **Predicates**: Functions that return true or false for given objects (e.g., $P(x)$ could mean "x is a prime number").  

Example of a formalized statement in FOL:  
$$
\forall x \ (Human(x) \rightarrow Mortal(x))
$$  
("All humans are mortal.")  

---

## **3. Formalization of Arguments**  
### **Logical Validity**  
An argument consists of premises and a conclusion. It is **valid** if, whenever the premises are true, the conclusion must also be true.  

#### **Common Rules of Inference**  
1. **Modus Ponens**:  
   If $P \rightarrow Q$ and $P$ is true, then $Q$ must be true.  
   $$
   P \rightarrow Q, \quad P \quad \therefore Q
   $$  
2. **Modus Tollens**:  
   If $P \rightarrow Q$ and $Q$ is false, then $P$ must be false.  
   $$
   P \rightarrow Q, \quad \neg Q \quad \therefore \neg P
   $$  
3. **Disjunctive Syllogism**:  
   If $P \lor Q$ is true and $\neg P$ is true, then $Q$ must be true.  
   $$
   P \lor Q, \quad \neg P \quad \therefore Q
   $$  

### **Formal Proofs**  
Proofs in logic use a step-by-step application of inference rules to derive conclusions from premises. **Truth tables**, **natural deduction**, and **proof by contradiction** are common proof methods.  

---

## **4. Applications in Mathematics and Computation**  
### **Mathematical Applications**  
- **Set theory**: Using logic to define and manipulate sets and their relationships.  
- **Proof verification**: Ensuring mathematical theorems are logically sound.  
- **Boolean algebra**: The foundation of logic gates in digital circuits.  

### **Computational Applications**  
- **Artificial Intelligence**: Logical reasoning underpins knowledge representation and automated decision-making.  
- **Formal Verification**: Checking the correctness of software and hardware.  
- **Programming Languages**: Logic programming (e.g., Prolog) is based on declarative reasoning.  

This foundational understanding of logic is essential for advanced topics in mathematical logic, theoretical computer science, and automated reasoning systems.
