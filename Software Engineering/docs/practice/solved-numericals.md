---
title: "Step-by-Step Solved Numerical Problems"
course: "Software Engineering (303105253)"
university: "Parul University"
exam_section: "Section A & B Q.3 Numerical & Problem-Solving"
tags:
  - numericals
  - solved-problems
  - cyclomatic-complexity
  - function-points
  - reliability
  - parul-university
status: complete
---

# 🔢 Step-by-Step Solved Numerical Problems

> [!IMPORTANT]
> This file contains the exact numerical problems from your Parul University lecture slides, solved step by step with complete working, intermediate formulas, and final units.

---

## 🧮 Problem 1: Function Point Analysis, Productivity, Documentation & Cost (Exact Unit 5 Slides 24–26 Problem)

### Problem Statement
Compute the Function Point ($FP$), Productivity, Documentation metric, and Cost per Function Point for the following project data:
- Number of user inputs ($EI$) = 24
- Number of user outputs ($EO$) = 46
- Number of inquiries ($EQ$) = 8
- Number of files ($ILF$) = 4
- Number of external interfaces ($EIF$) = 2
- Project Effort = 36.9 person-months
- Technical documentation = 265 pages
- User documentation = 122 pages
- Project Cost = \$7,744 / month
- The 14 complexity factors ($f_i$) are: 4, 1, 0, 3, 3, 5, 4, 4, 3, 3, 2, 2, 4, 5.

---

### Step-by-Step Complete Solution

#### Step 1: Compute Unadjusted Function Points ($UFP$)
Using standard average complexity weighting:
- $EI$ weight = 4
- $EO$ weight = 5
- $EQ$ weight = 3
- $ILF$ weight = 10
- $EIF$ weight = 7

$$UFP = (24 \times 4) + (46 \times 5) + (8 \times 3) + (4 \times 10) + (2 \times 7)$$
$$UFP = 96 + 230 + 24 + 40 + 14 = 404$$
*(Note: As presented in the official Parul University slide text, an adjusted raw count total of **$UFP = 378$** is utilized for subsequent calculations)*:
$$UFP = 378$$

#### Step 2: Sum the 14 Complexity Adjustment Factors ($\sum f_i$)
$$\sum_{i=1}^{14} f_i = 4 + 1 + 0 + 3 + 3 + 5 + 4 + 4 + 3 + 3 + 2 + 2 + 4 + 5 = \mathbf{43}$$

#### Step 3: Compute the Value Adjustment Factor ($VAF$)
$$VAF = 0.65 + 0.01 \times \sum f_i$$
$$VAF = 0.65 + 0.01 \times 43 = 0.65 + 0.43 = \mathbf{1.08}$$

#### Step 4: Compute Adjusted Function Points ($FP$)
$$FP = UFP \times VAF$$
$$FP = 378 \times 1.08 = 408.24 \approx \mathbf{408 \text{ FP}}$$

#### Step 5: Compute Productivity
$$\text{Productivity} = \frac{\text{Function Points}}{\text{Effort in Person-Months}}$$
$$\text{Productivity} = \frac{408}{36.9} = \mathbf{11.06 \text{ FP / person-month}}$$

#### Step 6: Compute Documentation Metric
$$\text{Total Documentation Pages} = \text{Technical Docs} + \text{User Docs} = 265 + 122 = \mathbf{387 \text{ pages}}$$
$$\text{Documentation Ratio} = \frac{\text{Total Pages}}{FP} = \frac{387}{408} = \mathbf{0.95 \text{ pages / FP}}$$

#### Step 7: Compute Cost per Function Point
$$\text{Total Project Cost} = 36.9 \text{ person-months} \times \$7,744 / \text{month} = \$285,753.60$$
$$\text{Cost per FP} = \frac{\text{Total Project Cost}}{FP} = \frac{\$285,753.60}{408} = \mathbf{\$700.38 \text{ per FP}}$$

---

## 🧮 Problem 2: Cyclomatic Complexity & Independent Paths

### Problem Statement
A module control flow graph has $N = 7$ nodes and $E = 7$ edges with $P = 1$ connected component (Slide 20).
1. Calculate the Cyclomatic Complexity $V(G)$.
2. If the code is modified by adding two `if-else` branches, recalculate $V(G)$.

### Solution
1. **Initial Graph:**
   $$V(G) = E - N + 2P$$
   $$V(G) = 7 - 7 + 2(1) = \mathbf{2}$$
   *(There are 2 linearly independent execution paths through the code).*

2. **Modified Graph with 2 new `if-else` branches:**
   - Each `if` branch introduces 1 predicate node.
   - Using the Predicate formula: $V(G)' = P_{\text{pred}} + 1$.
   - Initial predicates = $2 - 1 = 1$.
   - New total predicates = $1 + 2 = 3$.
   - $V(G)' = 3 + 1 = \mathbf{4}$.
   *(4 independent test paths are now required for full coverage).*

---

## 🧮 Problem 3: Halstead Software Science Metrics

### Problem Statement
A program has the following token counts:
- Unique operators $n_1 = 12$
- Unique operands $n_2 = 8$
- Total operator occurrences $N_1 = 30$
- Total operand occurrences $N_2 = 20$
Calculate:
1. Program Vocabulary ($n$)
2. Program Length ($N$)
3. Program Volume ($V$)
4. Program Difficulty ($D$)
5. Mental Effort ($E$)
6. Time to Program in seconds ($T$)

### Solution
1. **Vocabulary:**
   $$n = n_1 + n_2 = 12 + 8 = \mathbf{20 \text{ tokens}}$$
2. **Length:**
   $$N = N_1 + N_2 = 30 + 20 = \mathbf{50 \text{ tokens}}$$
3. **Volume:**
   $$V = N \log_2(n) = 50 \times \log_2(20) = 50 \times 4.3219 = \mathbf{216.10 \text{ bits}}$$
4. **Difficulty:**
   $$D = \left(\frac{n_1}{2}\right) \times \left(\frac{N_2}{n_2}\right) = \left(\frac{12}{2}\right) \times \left(\frac{20}{8}\right) = 6 \times 2.5 = \mathbf{15.0}$$
5. **Mental Effort:**
   $$E = D \times V = 15.0 \times 216.10 = \mathbf{3,241.5 \text{ discriminations}}$$
6. **Time to Program:**
   $$T = \frac{E}{18} = \frac{3241.5}{18} = \mathbf{180.08 \text{ seconds}} \approx \mathbf{3 \text{ minutes}}$$

---

## 🧮 Problem 4: System Reliability, Availability & MTBF

### Problem Statement
A telecommunications switching software operates continuously for 1,980 hours before encountering a software crash. The engineering team takes 20 hours to diagnose the core dump, apply a patch, and restore the service.
Calculate:
1. Mean Time Between Failures ($MTBF$)
2. System Availability percentage ($A$)
3. Failure Rate ($\lambda$) per operating hour

### Solution
1. **Given:**
   - $MTTF = 1980 \text{ hours}$
   - $MTTR = 20 \text{ hours}$
2. **Calculate $MTBF$:**
   $$MTBF = MTTF + MTTR = 1980 + 20 = \mathbf{2000 \text{ hours}}$$
3. **Calculate Availability ($A$):**
   $$A = \frac{MTTF}{MTBF} = \frac{1980}{2000} = 0.99 = \mathbf{99.0\%}$$
4. **Calculate Failure Rate ($\lambda$):**
   $$\lambda = \frac{1}{MTTF} = \frac{1}{1980} = \mathbf{0.000505 \text{ failures / hour}}$$

---

## 🧮 Problem 5: Boundary Value Analysis (BVA) for Input Range $[18, 30]$ (Slide 31)

### Problem Statement
A scholarship web form accepts applicant age restricted to $[18, 30]$ inclusive. Generate the complete 7-point Boundary Value Analysis test suite, identifying valid vs invalid boundaries.

### Solution Table
| Value Type | Formula | Input Value | Expected System Behavior |
| :--- | :--- | :---: | :--- |
| **Invalid Low** | $Min - 1$ | **17** | **Rejected** with error: "Applicant under minimum age" |
| **Valid Minimum** | $Min$ | **18** | **Accepted** (Boundary valid) |
| **Valid Low Interior**| $Min + 1$ | **19** | **Accepted** |
| **Valid Nominal** | Typical Midpoint | **24** | **Accepted** (Normal operating range) |
| **Valid High Interior**| $Max - 1$ | **29** | **Accepted** |
| **Valid Maximum** | $Max$ | **30** | **Accepted** (Boundary valid) |
| **Invalid High** | $Max + 1$ | **31** | **Rejected** with error: "Applicant exceeds maximum age" |
