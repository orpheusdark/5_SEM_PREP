# ⚡ Last-Minute Exam Revision & 30-Minute Cram Guide

[![Status](https://img.shields.io/badge/Cram%20Time-30%20Minutes-red.svg)](#)
[![Format](https://img.shields.io/badge/High%20Yield-Ultra%20Dense-yellow.svg)](#)

> [!IMPORTANT]
> **READ THIS IN THE FINAL 30 TO 60 MINUTES BEFORE ENTERING THE EXAM HALL!**  
> This sheet distills 321 lecture slides into ultra-dense, high-yield exam points, mandatory formulas, core definitions, and commonly tested distinctions.

---

## ⏱️ Final 30-Minute High-Yield Blitz (Read First!)

### 1. 🧮 The 5 Mathematical Formulas Guaranteed to Appear
1. **McCabe's Cyclomatic Complexity:**
   $$V(G) = E - N + 2P = P_{\text{pred}} + 1$$
   *(Where $E = \text{edges}, N = \text{nodes}, P = \text{connected components (usually 1)}, P_{\text{pred}} = \text{predicate/decision nodes})$.*
   *Trap Note:* Compound boolean conditions like `if (A && B)` count as **two** predicates!

2. **Albrecht's Function Point Formula:**
   $$FP = UFP \times [0.65 + 0.01 \times \sum_{i=1}^{14} f_i]$$
   *(Where $UFP = \sum (\text{Count} \times \text{Weight})$ across EI, EO, EQ, ILF, EIF; $f_i = 14$ GSC factors rated 0 to 5).*

3. **Halstead Program Volume & Effort:**
   $$\text{Vocabulary: } n = n_1 + n_2, \quad \text{Length: } N = N_1 + N_2$$
   $$\text{Volume: } V = N \log_2(n), \quad \text{Difficulty: } D = \left(\frac{n_1}{2}\right) \times \left(\frac{N_2}{n_2}\right), \quad \text{Effort: } E = D \times V$$
   $$\text{Time to Program: } T = \frac{E}{18} \text{ seconds (Stroud divisor = 18)}$$

4. **Software System Reliability & Availability:**
   $$MTBF = MTTF + MTTR, \quad \text{Availability } A = \frac{MTTF}{MTTF + MTTR} = \frac{MTTF}{MTBF}$$
   $$\text{Failure Rate } \lambda = \frac{1}{MTTF}$$

5. **Software Risk Exposure ($RE$):**
   $$RE = P \times I \quad (\text{Probability } \times \text{Financial/Schedule Impact})$$

---

### 2. ⚖️ High-Yield Distinctions Matrix (Exam Classics)

| Comparison | Core Difference / Definition | Critical Exam Keywords |
| :--- | :--- | :--- |
| **Verification vs. Validation** | Verification: *"Are we building the product right?"* (Conforms to specs).<br>Validation: *"Are we building the right product?"* (Satisfies user need). | Static vs Dynamic; Specs vs User intent; Developer vs Customer view. |
| **Coupling vs. Cohesion** | Coupling: *Inter-module* interdependence (Keep it **LOW**).<br>Cohesion: *Intra-module* functional strength (Keep it **HIGH**). | "Golden Rule: High Cohesion, Low Coupling"; Independence vs Single Purpose. |
| **Stub vs. Driver** | Stub: Dummy module called *by* module under test (Top-Down).<br>Driver: Test harness that *calls* module under test (Bottom-Up). | Top-Down Integration vs Bottom-Up Integration; Callee vs Caller. |
| **White-Box vs. Black-Box** | White-Box: Tests internal code logic, paths, conditions.<br>Black-Box: Tests input/output behavior against functional specs. | Glass-box/Structural vs Behavioral/Functional; Code visible vs Code invisible. |
| **Alpha vs. Beta Testing** | Alpha: Conducted at developer's site by users with developers.<br>Beta: Conducted at end-user's site in live, uncontrolled environment. | Developer site vs Client site; Controlled vs Uncontrolled environment. |
| **QA vs. QC** | Quality Assurance (QA): Process-oriented prevention of defects.<br>Quality Control (QC): Product-oriented detection of defects. | Prevention vs Detection; Process audit vs Testing/Inspection. |
| **Hard vs. Soft Real-Time** | Hard: Missing timing deadline is **catastrophic** (fatal).<br>Soft: Missing timing deadline causes **performance degradation**. | Deadlines strictly enforced; Human life/ABS vs Video streaming/Gaming. |

---

## 🏛️ Unit-by-Unit Essential Cheat Sheets

### Unit 1: Introduction & Process Models
- **Software Definition:** $\text{Software} = \text{Instructions} + \text{Data Structures} + \text{Documentation}$.
- **Software Crisis (NATO 1968):** Inability to deliver reliable software on time and within budget.
- **Bathtub Curve Trap:** Hardware exhibits bathtub wear-out (friction, rust); <mark>**Software does NOT wear out**</mark>, it **deteriorates** due to side-effects of maintenance patches.
- **Layered Tech (Q-P-M-T):** Quality Focus (bedrock) $\rightarrow$ Process $\rightarrow$ Methods $\rightarrow$ Tools.
- **4 Types of Maintenance (C-A-P-P):** Corrective (20% - bug fix), Adaptive (25% - environment change), Perfective (50% - new user features), Preventive (5% - refactoring).
- **Process Models Summary:**
  - *Waterfall:* Linear sequential; strictly fixed requirements; no working software until end.
  - *V-Model:* Verification (spec/design) mapped to Validation (unit/integration/system testing).
  - *Incremental:* Core product first, subsequent releases add features.
  - *RAD:* 60–90 days rapid delivery; component-heavy; requires multiple teams.
  - *Prototyping:* When requirements are vague; quick mockup evaluated by customer.
  - *Spiral (Barry Boehm):* Risk-driven; 4 quadrants: Planning, Risk Analysis, Engineering, Evaluation.
  - *Agile/Scrum:* 4 values (Individuals, Working software, Customer collaboration, Responding to change); 4 ceremonies (Planning, Daily Standup, Review, Retrospective); 3 roles (Product Owner, Scrum Master, Dev Team).

### Unit 2: Software Project Management
- **The 4 P's (Management Spectrum):** People (most critical), Product (scope & goals), Process (SDLC activities), Project (planning & control).
- **Barry Boehm's W5HH (7 Questions):** Why (business reason), What (scope), When (schedule), Who (roles), Where (location), How (strategy), How Much (resources: people, budget, space).
- **RMMM Plan:** Risk Mitigation (prevention), Risk Monitoring (tracking), Risk Management (contingency disaster recovery).
- **Team Structures:** Democratic Decentralized (consensus, research), Controlled Centralized (Chief Programmer, routine tasks), Controlled Decentralized (hierarchical).

### Unit 3: Requirements Engineering
- **5 RE Phases:** Feasibility Study $\rightarrow$ Elicitation $\rightarrow$ Specification $\rightarrow$ Validation $\rightarrow$ Management.
- **Feasibility Dimensions (T-O-E):** Technical, Operational, Economic feasibility.
- **SRS Characteristics (IEEE 830):** Concise, Unambiguous, Complete, Consistent, Verifiable, Modifiable, Traceable.
- **Functional vs. Non-Functional:** Functional = *What* it does (e.g., login, billing); Non-functional = *How well* it performs (latency < 2s, 99.99% uptime, AES-256).
- **Use Case Relationships:**
  - `<<include>>`: Mandatory shared logic. Base $\rightarrow$ Included.
  - `<<extend>>`: Optional/exceptional logic. Extension $\rightarrow$ Base.
- **Peter Chen ERD (1976):** Entity (Rectangle), Weak Entity (Double Rectangle), Attribute (Ellipse), Derived Attribute (Dashed Ellipse), Multi-valued (Double Ellipse), Key (Underlined), Relationship (Diamond).

### Unit 4: Structured System Design
- **Core Concepts:** Abstraction (procedural & data), Modularity, Architecture, Stepwise Refinement (Wirth), Information Hiding (Parnas), Refactoring.
- **Architectural Styles:** Data-Centered (Blackboard/Repository), Data-Flow (Pipe & Filter), Call-and-Return (Main/Subroutine), Layered (N-Tier: UI, Logic, DB), Object-Oriented.
- **ATAM:** Architecture Tradeoff Analysis Method (9 steps, evaluates Quality Attribute Utility Tree, tradeoff points).
- **Coupling Scale (Best to Worst):** No Direct $\rightarrow$ Data $\rightarrow$ Stamp $\rightarrow$ Control $\rightarrow$ External $\rightarrow$ Common $\rightarrow$ Content.
- **Cohesion Scale (Best to Worst):** Functional $\rightarrow$ Sequential $\rightarrow$ Communicational $\rightarrow$ Procedural $\rightarrow$ Temporal $\rightarrow$ Logical $\rightarrow$ Coincidental.

### Unit 5: Coding and Unit Testing
- **SOLID:** Single Responsibility, Open/Closed, Liskov Substitution, Interface Segregation, Dependency Inversion.
- **Principles:** KISS (Keep simple), DRY (Don't repeat), YAGNI (You aren't gonna need it).
- **Fagan Inspection (6 Stages):** Planning $\rightarrow$ Overview $\rightarrow$ Preparation $\rightarrow$ Inspection Meeting $\rightarrow$ Rework $\rightarrow$ Follow-up.
- **Cyclomatic Complexity:** $V(G) = E - N + 2P = P_{\text{pred}} + 1$.
- **Function Point Analysis:** 5 parameters (EI, EO, EQ, ILF, EIF); $FP = UFP \times [0.65 + 0.01 \times \sum f_i]$.
- **Halstead Metrics:** $n_1, n_2, N_1, N_2$; $N = N_1 + N_2$; $n = n_1 + n_2$; $V = N \log_2(n)$; $D = (n_1/2) \times (N_2/n_2)$; $E = D \times V$; $T = E / 18$.
- **Knot Count:** Formal intersection of control transfer arrows. Clean code has Knot Count = 0.

### Unit 6: Software Testing & Quality Assurance
- **Psychology of Testing:** Intent is to find errors; developers shouldn't test their own code.
- **Levels:** Unit $\rightarrow$ Integration (Top-down stubs, Bottom-up drivers, Regression, Smoke) $\rightarrow$ System $\rightarrow$ Acceptance (Alpha & Beta).
- **IEEE 829 Test Plan (8 Steps):** Analyze product, Strategy, Scope, Logistics, Objectives, Criteria (Entry/Suspension/Exit), Resources, Schedule.
- **BVA (Range $[18, 30]$):** 7 values: 17 (Min-1), 18 (Min), 19 (Min+1), 24 (Nominal), 29 (Max-1), 30 (Max), 31 (Max+1).
- **Pairwise Testing:** Orthogonal arrays; tests all pairs; reduces $> 4000$ cases down by $> 90\%$.
- **McCall's 11 Quality Factors:**
  - *Product Operation:* Correctness, Reliability, Efficiency, Integrity, Usability.
  - *Product Revision:* Maintainability, Flexibility, Testability.
  - *Product Transition:* Portability, Reusability, Interoperability.
- **ISO 9000 & 9001:** Quality Management System; 7-step certification process.

### Unit 7: CASE Tools & Dependability
- **CASE Tools:** Central Repository connects Upper CASE (planning/design) and Lower CASE (code/test).
- **Scrum CASE integration:** Sprint backlogs, user stories, burndown charts.
- **Dependability (5 Dimensions):** Reliability, Availability, Safety, Security, Resilience.
- **SRE Metrics:** $MTBF = MTTF + MTTR$; Availability $A = \frac{MTTF}{MTBF}$; Failure Rate $\lambda = 1/MTTF$.
- **Safety vs. Security:** Safety = harm prevention (hazard analysis, fail-safe); Security = CIA triad (Confidentiality, Integrity, Availability).

### Unit 8: Advanced Software Engineering
- **Software Reuse:** Benefits (dependability, low risk, speed); Problems (NIH syndrome, maintenance, tool lack); 4 levels (Application, Component, Library, Pattern).
- **CBSE 4 Framework Activities:** Qualification $\rightarrow$ Adaptation $\rightarrow$ Composition $\rightarrow$ Evolution.
- **Component Contracts:** Provides Interface (lollipop `---O`), Requires Interface (socket `---(`).
- **Distributed SE:** Client-Server (2-tier, 3-tier, N-tier) and Peer-to-Peer (P2P).
- **SOSE:** SOA, RESTful APIs (HTTP GET/POST/PUT/DELETE + JSON) vs. SOAP (XML).
- **Real-Time SE:** Hard Real-Time (fatal disaster if deadline missed) vs. Soft Real-Time (buffering/sluggishness). Rate Monotonic & Earliest Deadline First scheduling.
