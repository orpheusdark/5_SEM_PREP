# 📐 Software Engineering Formulas, Laws & Quick-Reference Sheet

[![Format](https://img.shields.io/badge/Formulas-LaTeX%20%26%20KaTeX-blue.svg)](#)
[![Parul University](https://img.shields.io/badge/Course-SE%20(303105253)-green.svg)](#)

---

## 1. 🧮 Cyclomatic Complexity Metrics (Thomas J. McCabe, 1976)

### Formulas
1. **Edge-Node Formula:**
   $$V(G) = E - N + 2P$$
   - $E$: Number of directed edges in the Control Flow Graph (CFG)
   - $N$: Number of nodes in CFG
   - $P$: Number of connected components (for a single monolithic procedure, $P = 1$)

2. **Predicate Node Formula:**
   $$V(G) = P_{\text{pred}} + 1$$
   - $P_{\text{pred}}$: Number of decision/predicate nodes (e.g., `if`, `while`, `for`, `case` branches).
   - <mark>**Crucial Exam Rule:**</mark> Compound conditions like `if (A && B)` count as **two** predicates!

3. **Planar Enclosed Regions Formula:**
   $$V(G) = R$$
   - $R$: Number of enclosed regions inside the planar graph $+ 1$ (the infinite outer region).

### Complexity Interpretation Table
| $V(G)$ Value | Risk Level | Software Testability |
| :---: | :---: | :--- |
| **1 – 10** | 🟢 Low Risk | Simple program; highly testable; easy to maintain. |
| **11 – 20** | 🟡 Moderate Risk | Moderately complex; requires thorough test suites. |
| **21 – 50** | 🟠 High Risk | Highly complex; error-prone; refactoring recommended. |
| **> 50** | 🔴 Untestable | Completely unstructured spaghetti code; cannot be tested safely. |

---

## 2. 🧮 Function Point Analysis (FPA — Allan Albrecht, IBM, 1979)

### 1. Functional Complexity Weights Table
| Functional Unit | Low | Average | High |
| :--- | :---: | :---: | :---: |
| **External Inputs (EI)** | 3 | **4** | 6 |
| **External Outputs (EO)** | 4 | **5** | 7 |
| **External Inquiries (EQ)** | 3 | **3** | 6 |
| **Internal Logical Files (ILF)** | 7 | **10** | 15 |
| **External Interface Files (EIF)** | 5 | **7** | 10 |

### 2. Formulas
1. **Unadjusted Function Points ($UFP$):**
   $$UFP = \sum_{i=1}^5 (\text{Count}_i \times \text{Weight}_i)$$

2. **Value Adjustment Factor ($VAF$):**
   Based on 14 General System Characteristics ($f_i$) scored 0 (no influence) to 5 (strong influence):
   $$VAF = 0.65 + 0.01 \times \sum_{i=1}^{14} f_i$$
   *(Range of $VAF$: $0.65 \le VAF \le 1.35$)*

3. **Adjusted Function Points ($FP$):**
   $$FP = UFP \times VAF = UFP \times \left[0.65 + 0.01 \times \sum_{i=1}^{14} f_i\right]$$

4. **Derived Project Metrics:**
   - **Productivity:** $\text{Productivity} = \frac{FP}{\text{Effort (Person-Months)}}$
   - **Cost per FP:** $\text{Cost/FP} = \frac{\text{Total Project Cost}}{\text{Total FP}}$
   - **Documentation Ratio:** $\text{Doc/FP} = \frac{\text{Total Documentation Pages}}{\text{Total FP}}$

---

## 3. 🧮 Halstead Software Science Metrics (Maurice Halstead, 1977)

### Primitive Parameters
- $n_1$: Count of **unique operators** (keywords, arithmetic, logical symbols: `if`, `while`, `+`, `=`, `;`)
- $n_2$: Count of **unique operands** (variables, constants, strings: `x`, `sum`, `3.14`, `"hello"`)
- $N_1$: Count of **total occurrences of operators**
- $N_2$: Count of **total occurrences of operands**

### Formulas
| Metric Name | Symbol | Exact Formula | Unit |
| :--- | :---: | :--- | :---: |
| **Program Vocabulary** | $n$ | $n = n_1 + n_2$ | Unique tokens |
| **Total Program Length** | $N$ | $N = N_1 + N_2$ | Total tokens |
| **Calculated Length** | $\hat{N}$ | $\hat{N} = n_1 \log_2(n_1) + n_2 \log_2(n_2)$ | Estimated tokens |
| **Program Volume** | $V$ | $V = N \log_2(n)$ | Bits |
| **Program Difficulty** | $D$ | $D = \left(\frac{n_1}{2}\right) \times \left(\frac{N_2}{n_2}\right)$ | Ratio |
| **Program Effort** | $E$ | $E = D \times V$ | Elementary mental discriminations |
| **Time to Program** | $T$ | $T = \frac{E}{18}$ | Seconds (Stroud number $S=18$) |

---

## 4. 🧮 Software Reliability & Availability Metrics

| Metric | Symbol | Formula | Meaning |
| :--- | :---: | :--- | :--- |
| **Mean Time Between Failures** | $MTBF$ | $MTBF = MTTF + MTTR$ | Total average cycle time between breakdowns. |
| **System Availability** | $A$ | $A = \frac{MTTF}{MTBF} = \frac{MTTF}{MTTF + MTTR}$ | Operational uptime proportion (e.g., 0.999 = 99.9%). |
| **Failure Rate** | $\lambda$ | $\lambda = \frac{1}{MTTF}$ | Frequency of failures per operating hour. |
| **Annual Downtime** | $D_{\text{annual}}$ | $D = (1 - A) \times 8760 \text{ hours}$ | Total hours system is dead per year. |

---

## 5. 🪢 Knot Count Metric (Unstructured Code Detection)
- Line jump pair: $(a, b)$ representing transfer of control from line $a$ to line $b$.
- Two jumps $(a, b)$ and $(p, q)$ intersect to form a **Knot** if:
  $$\min(a,b) < \min(p,q) < \max(a,b) \quad \text{and} \quad \max(p,q) > \max(a,b)$$
  $$\text{OR}$$
  $$\min(a,b) < \max(p,q) < \max(a,b) \quad \text{and} \quad \min(p,q) < \min(a,b)$$
- *Rule:* Well-structured code has a **Knot Count = 0**.

---

## 6. 📐 Coupling & Cohesion Reference Hierarchies

### Cohesion Hierarchy (Strive for HIGHEST)
1. **Functional (Best):** Single well-defined mathematical or logical function (`sin(x)`).
2. **Sequential:** Output of one step is direct input to the next step.
3. **Communicational:** Functions operate on the exact same input/output data.
4. **Procedural:** Functions follow a specific sequence of execution.
5. **Temporal:** Functions execute at the same moment in time (e.g., startup).
6. **Logical:** Functions perform similar categories of operations chosen by a flag.
7. **Coincidental (Worst):** Completely unrelated tasks grouped together randomly.

### Coupling Hierarchy (Strive for LOWEST)
1. **No Direct (Best):** Modules do not communicate directly.
2. **Data:** Modules communicate via simple primitive parameters (`int`, `float`).
3. **Stamp:** Modules pass entire composite records/structs when only part is needed.
4. **Control:** One module passes a flag that alters the internal logic of another.
5. **External:** Modules tied to external device protocols or OS interfaces.
6. **Common:** Modules read and write to shared global data/variables.
7. **Content (Worst):** One module directly accesses or branches into another's internals.

---

## 7. 📜 Software Engineering Standards Reference
- **IEEE 830:** Standard for Software Requirements Specification (SRS).
- **IEEE 829:** Standard for Software Test Documentation (Test Plans, Test Cases).
- **ISO 9000:** Quality Management Concepts and Vocabulary.
- **ISO 9001:** Requirements for a Quality Management System (QMS).
- **SEI CMMI:** Capability Maturity Model Integration (Levels 1 to 5: Initial, Managed, Defined, Quantitatively Managed, Optimizing).
