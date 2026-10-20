---
title: "Short-Answer Questions & Model Solutions (2 Marks)"
course: "Software Engineering (303105253)"
university: "Parul University"
exam_section: "Section A & B Q.1 Compulsory Questions"
tags:
  - short-answers
  - 2-marks
  - parul-university
status: complete
---

# 📝 Section A & B Q.1 Model Short Answers (2 Marks Each)

> [!TIP]
> **HOW TO SCORE FULL 2/2 MARKS:**
> Write exactly 2–3 precise bullet points containing the **essential technical keywords**. Parul University examiners look for exact keywords!

---

### Q1-1: Define Software Engineering according to IEEE.
**Model Answer:**
Software Engineering is defined by IEEE as:
1. The application of a **systematic, disciplined, and quantifiable approach** to the development, operation, and maintenance of software; that is, the application of engineering to software.
2. The study of approaches as in (1).
- *Essential Formula:* $\text{Software} = \text{Instructions} + \text{Data Structures} + \text{Documentation}$.

---

### Q1-2: What is the Software Crisis? State two primary causes.
**Model Answer:**
The **Software Crisis** (NATO Conference, 1968) refers to the inability of the software industry to deliver reliable, functional software on time and within budget.
- *Causes:*
  1. Rapid increase in hardware computing power and system complexity without structured engineering methods.
  2. Lack of formal requirements elicitation leading to continuous unmanaged scope changes.

---

### Q1-3: What is the difference between Verification and Validation?
**Model Answer:**
- **Verification:** Evaluates intermediate work products to determine whether they meet requirements specified at the start of that phase. (*"Are we building the product right?"* — Static reviews, inspections).
- **Validation:** Evaluates the final operational software to ensure it satisfies customer business needs. (*"Are we building the right product?"* — Dynamic execution, acceptance testing).

---

### Q2-1: Name the 4 P's in the Software Management Spectrum.
**Model Answer:**
1. **People:** The most critical asset; includes managers, developers, clients, and end users.
2. **Product:** The software objectives, scope, and problem decomposition.
3. **Process:** The framework of activities (SDLC model) chosen to deliver the product.
4. **Project:** All planning, tracking, resource allocation, and risk management activities.

---

### Q2-2: Define Barry Boehm's W5HH principle.
**Model Answer:**
The W5HH principle is a management framework proposed by Dr. Barry Boehm containing 7 fundamental questions to define project objectives:
- **Why** is the system being developed?
- **What** will be done?
- **When** will it be done?
- **Who** is responsible?
- **Where** are they located?
- **How** will the job be done technically?
- **How much** of each resource is needed?

---

### Q3-1: Distinguish between Functional and Non-Functional Requirements.
**Model Answer:**
- **Functional Requirements:** Define *what* services and behavior the software must perform (e.g., calculate sales tax, process user login).
- **Non-Functional Requirements:** Define *how well* the system performs its functions under operational constraints (e.g., response time $< 2$ seconds, 99.9% uptime, AES-256 encryption).

---

### Q3-2: In a Use Case Diagram, distinguish `<<include>>` from `<<extend>>`.
**Model Answer:**
- `<<include>>`: Represents **mandatory** sub-routine behavior that is *always executed* when the base use case runs (e.g., `Checkout` includes `Authenticate`).
- `<<extend>>`: Represents **optional** behavior that executes *only if specific conditional triggers occur* (e.g., `Order` extended by `Apply Discount Coupon`).

---

### Q4-1: State the Golden Rule of Software Design.
**Model Answer:**
The foundational design heuristic is to **Maximize Cohesion** and **Minimize Coupling**:
- *High Cohesion:* Keep elements inside a module strongly focused on a single responsibility.
- *Low Coupling:* Minimize dependencies and connections between distinct modules to reduce the ripple effect of bugs.

---

### Q4-2: Differentiate between Data Coupling and Stamp Coupling.
**Model Answer:**
- **Data Coupling (Best):** Modules communicate strictly by passing primitive scalar parameters (e.g., `calculate_area(float length, float width)`).
- **Stamp Coupling:** Modules communicate by passing an entire composite data structure/record when only a small subset of fields is needed (e.g., passing an entire `CustomerRecord` just to read `customer.zip_code`).

---

### Q5-1: State McCabe's Cyclomatic Complexity formula and its significance.
**Model Answer:**
$$V(G) = E - N + 2P = P_{\text{pred}} + 1$$
- *Parameters:* $E$ = edges, $N$ = nodes, $P$ = connected components, $P_{\text{pred}}$ = predicate nodes.
- *Significance:* Defines the exact number of **linearly independent basis paths** required to achieve 100% path coverage during white-box testing.

---

### Q5-2: What does a Knot Count of 0 indicate in program structure?
**Model Answer:**
A **Knot Count of 0** indicates that control transfer arrows do not cross or intersect in the program's control flow. This mathematically verifies that the code is **well-structured** and free from unstructured spaghetti jumps (`goto` statements).

---

### Q6-1: Differentiate between a Test Stub and a Test Driver.
**Model Answer:**
- **Test Stub:** A dummy routine that simulates a *called subordinate module*; used in **Top-Down Integration Testing**.
- **Test Driver:** A test harness script that *calls the module under test* with parameters; used in **Bottom-Up Integration Testing**.

---

### Q6-2: Distinguish between Alpha Testing and Beta Testing.
**Model Answer:**
- **Alpha Testing:** Conducted at the **developer's site** by representative end users in a controlled environment with developers present.
- **Beta Testing:** Conducted at **end-user sites** in a live, real-world uncontrolled operational environment without developers present.

---

### Q7-1: State the relationship between MTBF, MTTF, and MTTR.
**Model Answer:**
$$MTBF = MTTF + MTTR$$
- $MTTF$ (Mean Time To Failure): Operational uptime before breakdown.
- $MTTR$ (Mean Time To Repair): Downtime taken to restore the system.
- $MTBF$ (Mean Time Between Failures): Total cycle time between consecutive breakdowns.

---

### Q8-1: Differentiate between Hard Real-Time and Soft Real-Time systems.
**Model Answer:**
- **Hard Real-Time:** Missing a timing deadline results in **total catastrophic system failure** and potential loss of human life (e.g., airbag deployment, pacemaker).
- **Soft Real-Time:** Missing a timing deadline causes **performance degradation** and reduced quality of service, but no physical damage (e.g., video streaming buffering).
