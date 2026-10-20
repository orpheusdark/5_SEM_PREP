---
title: "Multiple Choice Questions (MCQs) & Trap Analysis"
course: "Software Engineering (303105253)"
university: "Parul University"
tags:
  - mcqs
  - practice
  - exam-preparation
status: complete
---

# 🧠 High-Yield Multiple Choice Questions & Trap Analysis

---

### Unit 1: Introduction & Process Models

#### Q1. Software is defined as:
- A) A collection of executable programs only.
- B) Programs + Data Structures + Documentation.
- C) Executable machine code + Operating System.
- D) User manuals and algorithms.

<details>
<summary><b>💡 Click to Reveal Correct Answer & Trap Analysis</b></summary>

**Correct Answer: B**

*Explanation:*

</details>
 By formal engineering definition, software consists of instructions (code), data structures that enable manipulation, and documents that describe its use.

#### Q2. Why does software NOT exhibit the classic hardware bathtub failure curve?
- A) Software is immune to any form of defects.
- B) Software has no physical components and deteriorates due to maintenance side-effects rather than physical wear.
- C) Software fails only during the first 30 days of release.
- D) Software failures are completely random and untraceable.

<details>
<summary><b>💡 Click to Reveal Correct Answer & Trap Analysis</b></summary>

**Correct Answer: B**

*Trap Explanation:*

</details>
 Hardware wears out due to physical friction and environmental degradation. Software deteriorates when maintenance changes cause uncoordinated side-effects.

#### Q3. In which SDLC model is explicit Risk Analysis conducted in a dedicated quadrant?
- A) Waterfall Model
- B) RAD Model
- C) Barry Boehm's Spiral Model
- D) Prototyping Model

<details>
<summary><b>💡 Click to Reveal Correct Answer & Trap Analysis</b></summary>

**Correct Answer: C**

*Explanation:*

</details>
 The Spiral Model is explicitly risk-driven, featuring a dedicated Risk Analysis quadrant (Quadrant 2).

#### Q4. What are the 4 bedrock layers of Software Engineering technology?
- A) Planning, Coding, Testing, Deployment
- B) A Quality Focus, Process, Methods, Tools
- C) Software, Hardware, Network, People
- D) Analysis, Design, Coding, Verification

<details>
<summary><b>💡 Click to Reveal Correct Answer & Trap Analysis</b></summary>

**Correct Answer: B (Mnemonic: Q-P-M-T)**



---



### Unit 2: Software Project Management



#### Q5. The 4 P's of the software management spectrum are:

- A) Planning, Programming, Performance, Profit

- B) People, Product, Process, Project

- C) Personnel, Program, Procedure, Plan

- D) Principle, Purpose, Practice, Product

**

</details>
Correct Answer: B**  
> *Explanation:* People (human capital), Product (objectives/scope), Process (SDLC activities), Project (planning/control).

#### Q6. If a risk has a probability of 0.40 and an impact cost of $50,000, its Risk Exposure ($RE$) is:
- A) $125,000
- B) $50,040
- C) $20,000
- D) $2,000

<details>
<summary><b>💡 Click to Reveal Correct Answer & Trap Analysis</b></summary>

**Correct Answer: C**

*Explanation:*

</details>
 $RE = P \times I = 0.40 \times 50,000 = \$20,000$.

---

### Unit 3: Requirements Engineering

#### Q7. Which IEEE standard defines the format and contents of a Software Requirements Specification (SRS)?
- A) IEEE 829
- B) IEEE 830
- C) IEEE 1074
- D) IEEE 1012

<details>
<summary><b>💡 Click to Reveal Correct Answer & Trap Analysis</b></summary>

**Correct Answer: B**

*Trap Note:*

</details>
 IEEE 829 is for Test Documentation; IEEE 830 is for SRS.

#### Q8. In a Use Case Diagram, an optional feature that executes only when a specific conditional trigger occurs is modeled using:
- A) `<<include>>`
- B) `<<extend>>`
- C) Generalization
- D) Aggregation

<details>
<summary><b>💡 Click to Reveal Correct Answer & Trap Analysis</b></summary>

**Correct Answer: B (`<<extend>>`)**



---



### Unit 4: Structured System Design



#### Q9. The ideal architectural design objective is to achieve:

- A) High Coupling and High Cohesion

- B) Low Coupling and Low Cohesion

- C) Low Coupling and High Cohesion

- D) High Coupling and Low Cohesion

**

</details>
Correct Answer: C (The Golden Rule: High Cohesion, Low Coupling)**

#### Q10. Two modules share a common global variable array in memory. What type of coupling exists between them?
- A) Data Coupling
- B) Stamp Coupling
- C) Common Coupling
- D) Content Coupling

<details>
<summary><b>💡 Click to Reveal Correct Answer & Trap Analysis</b></summary>

**Correct Answer: C (Common Coupling)**



#### Q11. Which type of cohesion is exhibited when a module performs a single, well-defined mathematical function like `compute_tangent(x)`?

- A) Functional Cohesion

- B) Communicational Cohesion

- C) Procedural Cohesion

- D) Logical Cohesion

**

</details>
Correct Answer: A (Functional Cohesion — the highest and best)**

---

### Unit 5: Coding, Metrics & Unit Testing

#### Q12. For a program control graph with 11 edges, 8 nodes, and 1 connected component, the Cyclomatic Complexity $V(G)$ is:
- A) 3
- B) 4
- C) 5
- D) 2

<details>
<summary><b>💡 Click to Reveal Correct Answer & Trap Analysis</b></summary>

**Correct Answer: C**

*Calculation:*

</details>
 $V(G) = E - N + 2P = 11 - 8 + 2(1) = 5$.

#### Q13. In Halstead's metrics, what is the Stroud number divisor used to calculate programming time in seconds?
- A) 60
- B) 3600
- C) 18
- D) 100

<details>
<summary><b>💡 Click to Reveal Correct Answer & Trap Analysis</b></summary>

**Correct Answer: C (18 elementary mental discriminations per second)**



---



### Unit 6: Software Testing & Quality Assurance



#### Q14. In Boundary Value Analysis for the valid range $[18, 30]$, which pair represents the **invalid** boundary test inputs?

- A) 18 and 30

- B) 19 and 29

- C) 17 and 31

- D) 24 and 25

**

</details>
Correct Answer: C ($Min - 1 = 17$ and $Max + 1 = 31$)**

#### Q15. In integration testing, a dummy routine that simulates a called sub-module is called a:
- A) Driver
- B) Stub
- C) Proxy
- D) Mock

<details>
<summary><b>💡 Click to Reveal Correct Answer & Trap Analysis</b></summary>

**Correct Answer: B (Stub — used in Top-Down integration)**



#### Q16. Which McCall quality factor measures the ease with which software can be transferred from Windows to Linux?

- A) Maintainability

- B) Interoperability

- C) Portability

- D) Reusability

**

</details>
Correct Answer: C (Portability)**

---

### Unit 7 & 8: CASE Tools & Advanced SE

#### Q17. A server experiences an $MTTF$ of 490 hours and an $MTTR$ of 10 hours. What is its Availability?
- A) 95.0%
- B) 98.0%
- C) 99.0%
- D) 99.9%

<details>
<summary><b>💡 Click to Reveal Correct Answer & Trap Analysis</b></summary>

**Correct Answer: B**

*Calculation:*

</details>
 $A = 490 / (490 + 10) = 490 / 500 = 0.98 = 98.0\%$.

#### Q18. Which of the following is a Hard Real-Time system?
- A) Online multiplayer video game
- B) Video streaming on Netflix
- C) Automotive anti-lock braking system (ABS)
- D) Web application search engine
> **Correct Answer: C (Missing deadline results in fatal car crash)**
