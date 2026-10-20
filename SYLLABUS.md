# 🗺️ Master Syllabus & Slide Traceability Map

[![Status](https://img.shields.io/badge/Coverage-100%25%20(321%20Slides)-brightgreen.svg)](#)
[![Parul University](https://img.shields.io/badge/Parul%20University-303105253-red.svg)](https://www.paruluniversity.ac.in)

> **Course Code:** Software Engineering (`303105253`)  
> **Target Audience:** B.Tech / Diploma / M.Tech Computer Science & Engineering Students  
> **Source Material:** All 8 official Parul University presentation decks (321 total slides) cross-referenced with Roger S. Pressman (*Software Engineering: A Practitioner's Approach*) and Ian Sommerville (*Software Engineering*).

---

## 📑 Slide Inventory Summary

| File Name | Unit / Module Title | Total Slides | Key Syllabus Coverage | Markdown Module Link |
| :--- | :--- | :---: | :--- | :---: |
| `SE unit 1.pdf` | **Unit 1: Introduction & Process Models** | 89 | Definition, Software Characteristics, Crisis, Layered Tech, Generic View, Models (Waterfall, V, Incremental, RAD, Prototyping, Spiral, Concurrent, Agile, XP, Scrum), UML Diagrams | [📖 View Unit 1](docs/units/unit-01-introduction-and-process-models.md) |
| `SE unit 2.pdf` | **Unit 2: Software Project Management** | 23 | Management Spectrum (4 Ps), W5HH Principle, Team Management, Risk Management (Identification, Assessment, Control), Project Monitoring & KPIs | [📖 View Unit 2](docs/units/unit-02-software-project-management.md) |
| `SE unit 3.pdf` | **Unit 3: Requirements Engineering** | 32 | Problem Recognition, RE Process, Feasibility Study, Elicitation, Specification (SRS), Functional vs Non-Functional, Validation, Use Cases (Include/Extend), DFD, ERD | [📖 View Unit 3](docs/units/unit-03-requirements-engineering.md) |
| `SE unit 4.pdf` | **Unit 4: Structured System Design** | 67 | Design Concepts (Abstraction, Modularity, Refinement, Hiding, Refactoring), Architectural Styles (Data-Centered, Pipe & Filter, Call/Return, Layered, OO), ATAM, Peter Chen ERD, DFD vs CFD, Coupling & Cohesion | [📖 View Unit 4](docs/units/unit-04-structured-system-design.md) |
| `SE unit 5.pdf` | **Unit 5: Coding & Unit Testing** | 34 | Programming Guidelines, Coding Standards, KISS/DRY/YAGNI, SOLID Principles, Unit Testing, Fagan Inspection, Cyclomatic Complexity, Function Point Analysis, Halstead Metrics, Knot Count | [📖 View Unit 5](docs/units/unit-05-coding-and-unit-testing.md) |
| `SE unit 6.pdf` | **Unit 6: Software Testing & SQA** | 53 | Quality Concepts, Psychology of Testing, Levels of Testing, Test Plan (IEEE 829), BVA, Pairwise Testing, State-Based Testing, SQA, McCall's Quality Factors, ISO 9000/9001 | [📖 View Unit 6](docs/units/unit-06-software-testing-and-quality-assurance.md) |
| `SE unit 7.pdf` | **Unit 7: CASE Tools & Dependability** | 11 | CASE Tools Architecture, Central Repository, Scrum Integration, System Dependability, SRE Metrics (MTTF, MTTR, MTBF, Availability), Safety, Security, Resilience | [📖 View Unit 7](docs/units/unit-07-case-tools-and-system-dependability.md) |
| `SE unit 8.pdf` | **Unit 8: Advanced Software Engineering** | 12 | Software Reuse, CBSE Lifecycle, Distributed SE (Client-Server, P2P), Service-Oriented SE (SOA, REST), Real-Time SE (Hard/Soft), Systems Engineering | [📖 View Unit 8](docs/units/unit-08-advanced-software-engineering.md) |

---

## 🔍 Detailed Slide-by-Slide Topic Breakdown

### 📦 Unit 1: Introduction & Process Models (89 Slides)
- **Slides 2–5:** Definition of Software Engineering: Framework for building software; systematic, disciplined, quantifiable approach. Software formula: $\text{Software} = \text{Instructions} + \text{Data Structures} + \text{Documents}$.
- **Slides 6–9:** The Software Crisis: Difficulties of delivering functional software on time and within budget. Common software myths and the importance of SE.
- **Slides 10–12:** Types of Software Engineers (Front-End, Back-End, Full-Stack) & Industry Applications (Mobile, Web, Embedded, AI/ML, Cloud).
- **Slides 13–18:** Software Characteristics: Engineered not manufactured; does not wear out (bathtub curve vs. software curve); custom-built. 4 Quality characteristics: Functionality, Reliability, Efficiency, Usability.
- **Slides 19–20:** Layered Technology: 4 layers — A Quality Focus, Process, Methods, Tools (Mnemonic: **Q-P-M-T**).
- **Slides 21–24:** Generic View of SE: Definition Phase ("What"), Development Phase ("How"), Support Phase ("Change"). **4 Maintenance Types:** Corrective (20%), Adaptive (25%), Perfective (50%), Preventive (5%).
- **Slides 25–27:** Waterfall Model: Linear sequential phases, pros, cons, and blocking states.
- **Slides 28–31:** V-Model: Verification (Requirements, System, Architecture, Module Design) vs. Validation (Unit, Integration, System, Acceptance testing).
- **Slides 32–35:** Incremental Process Model: Core product first, subsequent increments add functionality.
- **Slides 36–39:** Iterative Model: Cyclic development, drawbacks of iterative waterfall.
- **Slides 40–42:** RAD (Rapid Application Development) Model: 60–90 day lifecycle, component-based construction.
- **Slides 43–44:** Evolutionary Process Models: Combining iterative and incremental approaches.
- **Slides 45–50:** Prototyping Model: Communication, quick design, prototype construction, customer evaluation. Real-world analogy (Architect house plan).
- **Slides 51–55:** Spiral Model (Barry Boehm): Risk-driven process model. 4 quadrants (Planning, Risk Analysis, Engineering, Evaluation). Case study: Microsoft Windows OS development.
- **Slides 56–58:** Concurrent Development Model: Concurrent state transitions (under development, awaiting changes, under review, baseline). Aerospace application.
- **Slides 59–64:** Agile Development: Agility principles, Agile Manifesto values, rapid adaptation.
- **Slides 65–69:** Agile Methodologies: Scrum (Roles, Artifacts, Ceremonies), Extreme Programming (XP: Pair programming, continuous integration), Kanban Board (To Do, Doing, Done).
- **Slides 70–88:** Unified Modeling Language (UML):
  - *Structural Diagrams:* Class Diagram (Attributes, Methods, Relationships), Object Diagram, Component Diagram, Deployment Diagram.
  - *Behavioral Diagrams:* Use Case Diagram (Actors, Boundary), State Machine Diagram, Activity Diagram, Sequence Diagram (Lifelines, Messages).
  - *Case Study:* Railway Reservation Use Case Diagram.

---

### 📊 Unit 2: Software Project Management (23 Slides)
- **Slides 2–5:** SPM Definition: Art & discipline of planning, organizing, directing, and controlling software projects. The 3 Constraints: **Time, Cost, Quality**.
- **Slides 6–9:** The Management Spectrum (**4 P's**):
  - **People:** Stakeholders, team leaders, project team.
  - **Product:** Objectives, scope, problem decomposition.
  - **Process:** Framework and umbrella activities.
  - **Project:** Planning, monitoring, risk control.
- **Slides 10–13:** Barry Boehm's **W5HH Principle** (7 Questions):
  1. *Why* is the system being developed?
  2. *What* will be done?
  3. *When* will it be accomplished?
  4. *Who* is responsible?
  5. *Where* are they organizationally located?
  6. *How* will the job be done technically and managerially?
  7. *How much* of each resource is needed? (Human, Financial, Space).
- **Slide 14:** Importance of Team Management: Collaborative culture, communication, team coordination.
- **Slides 15–17:** Software Risk Management: Risk Identification, Risk Analysis, Risk Projection, Risk Assessment & Control (RMMM: Risk Mitigation, Monitoring, and Management).
- **Slides 18–22:** Project Monitoring Plan:
  - Key Performance Indicators (KPIs): Schedule Variance, Effort Variance.
  - Tools & Techniques: JIRA, Trello, Microsoft Project.
  - Risk registers, data collection, and milestone reporting.

---

### 📋 Unit 3: Requirements Engineering (32 Slides)
- **Slides 2–4:** Requirements Engineering Definition & 5-Step Process: Feasibility Study, Elicitation, Specification, Validation, Management.
- **Slide 5:** Feasibility Study Dimensions: Technical, Operational, Economic ($T-O-E$) Feasibility.
- **Slide 6:** Requirements Elicitation Techniques: Interviews, Questionnaires, FAST (Facilitated Application Specification Techniques), Brainstorming, Prototyping.
- **Slides 7–8:** Software Requirements Specification (SRS): Characteristics of a good SRS (Concise, Unambiguous, Complete, Consistent, Verifiable, Modifiable, Traceable) conforming to **IEEE 830**.
- **Slides 9–12:** Requirements Classification:
  - **Functional Requirements:** System features, calculations, data manipulation.
  - **Non-Functional Requirements:** Performance, Security, Usability, Reliability, Portability (FURPS+).
- **Slides 13–15:** Requirements Verification & Validation: Boehm's rule ("Have we got the requirements right?"). Requirements Management: Traceability matrix, change control.
- **Slides 16–20:** Use Case Modeling: Actors, System boundary, Use cases. Relationships:
  - `<<include>>`: Mandatory sub-routine functionality.
  - `<<extend>>`: Optional/conditional extension behavior.
  - Generalization: Inheritance among actors or use cases.
- **Slides 21–27:** Requirements Analysis & Modeling:
  - Context Diagram (Level 0 DFD): System as a single bubble with external entities.
  - DFD (Data Flow Diagram): Processes, Data Stores, Data Flows, External Entities.
  - Entity-Relationship Diagram (ERD): Entities, Relationships, Cardinality.
- **Slides 28–31:** Requirements Validation Techniques: Formal Requirement Reviews, Prototyping, Walkthroughs.

---

### 🏗️ Unit 4: Structured System Design (67 Slides)
- **Slides 2–10:** Fundamental Design Concepts:
  1. *Abstraction:* Procedural & Data Abstraction (Hiding irrelevant implementation details).
  2. *Modularity:* Subdividing a system into manageable modules (Meyer's criteria).
  3. *Architecture:* High-level structural framework.
  4. *Refinement:* Stepwise top-down refinement (Niklaus Wirth).
  5. *Design Patterns:* Reusable solutions to recurring problems.
  6. *Information Hiding:* David Parnas principle (Modules encapsulate internal details).
  7. *Refactoring:* Restructuring internal design without changing external behavior.
- **Slides 11–13:** The Design Model: Data design, Architectural design, Interface design, Component-level design.
- **Slides 14–25:** Architectural Styles & Patterns:
  - *Data-Centered Architecture:* Central repository / blackboard with independent client software.
  - *Data Flow Architecture:* Pipe and Filter pattern (Sequential transformation of streams).
  - *Call and Return Architecture:* Main program/subroutine, remote procedure calls.
  - *Object-Oriented Architecture:* Encapsulated data and operations.
  - *Layered Architecture (N-Tier):* Hierarchical layers; each provides services to the layer above.
- **Slides 26–31:** Alternative Architectural Designs & ATAM:
  - Architecture Trade-off Analysis Method (ATAM): 9-step evaluation of quality attributes (Performance vs Modifiability vs Security). Utility tree, sensitivity points, trade-off points.
- **Slides 32–36:** Object-Oriented Design (OOD): Objects, Classes, Abstraction, Encapsulation, Inheritance, Polymorphism.
- **Slides 37–52:** Data-Oriented Modeling (Peter Chen 1976 ER Model):
  - Strong Entities vs Weak Entities (Double rectangle, identifying relationship).
  - Attribute Types: Simple, Composite, Single-valued, Multi-valued (Double ellipse), Derived (Dashed ellipse), Key.
  - Cardinality & Modality: 1:1, 1:N, M:N.
- **Slides 53–57:** Dataflow Model: Logical DFD (Business view) vs Physical DFD (Implementation view).
- **Slides 58–61:** Control Flow Model (CFD): Control flow diagrams, Control Specification (C-Spec), Process Specification (P-Spec), Bug tracking lifecycle.
- **Slides 62–66:** **Coupling and Cohesion (The Golden Rule: High Cohesion, Low Coupling):**
  - **Coupling (Degree of Interdependence):**
    1. No Direct Coupling (Best)
    2. Data Coupling
    3. Stamp Coupling
    4. Control Coupling
    5. External Coupling
    6. Common Coupling
    7. Content Coupling (Worst)
  - **Cohesion (Internal Module Strength):**
    1. Functional Cohesion (Best)
    2. Sequential Cohesion
    3. Communicational Cohesion
    4. Procedural Cohesion
    5. Temporal Cohesion
    6. Logical Cohesion
    7. Coincidental Cohesion (Worst)

---

### 💻 Unit 5: Coding and Unit Testing (34 Slides)
- **Slides 2–8:** Coding Standards & Guidelines: Readability, safety, security, variable naming, line length limits (<= 80 characters).
- **Slides 9–12:** Programming Principles:
  - KISS (Keep It Simple, Stupid), DRY (Don't Repeat Yourself), YAGNI (You Aren't Gonna Need It).
  - SOLID Principles: Single Responsibility, Open/Closed, Liskov Substitution, Interface Segregation, Dependency Inversion.
- **Slide 13:** Unit Testing: Testing individual functional modules and classes in isolation.
- **Slides 14–16:** Code Inspection: Formal Fagan inspection process (Planning, Overview, Preparation, Inspection Meeting, Rework, Follow-up).
- **Slides 17–20:** **McCabe's Cyclomatic Complexity:**
  - Formula 1: $V(G) = E - N + 2P$ (where $E$ = edges, $N$ = nodes, $P$ = connected components, typically 1).
  - Formula 2: $V(G) = P_{\text{pred}} + 1$ (where $P_{\text{pred}}$ = number of predicate/decision nodes).
  - Slide Example: $N = 7, E = 7 \Rightarrow V(G) = 7 - 7 + 2(1) = 2$.
- **Slides 21–26:** **Function Point Analysis (Albrecht's FPA):**
  - 5 Information Domain Parameters: External Inputs (EI), External Outputs (EO), External Inquiries (EQ), Internal Logical Files (ILF), External Interface Files (EIF).
  - Formula: $FP = UFP \times [0.65 + 0.01 \times \sum f_i]$ where $\sum f_i$ is the sum of 14 General System Characteristics (GSCs).
  - **Slide 24–26 Exact Solved Problem:**
    - Inputs: 24 EI, 46 EO, 8 EQ, 4 ILF, 2 EIF.
    - $\sum f_i = 43$. Effort = 36.9 person-months. Technical docs = 265 pages, User docs = 122 pages. Cost = $7,744/month.
    - $UFP = 378, VAF = 0.65 + 0.01 \times 43 = 1.08, FP = 378 \times 1.08 = 408$.
    - Productivity = $408 / 36.9 = 11.06$ FP/person-month.
    - Documentation = $(265 + 122) / 408 = 0.94$ pages/FP.
    - Cost per FP = $(36.9 \times 7744) / 408 = \$700.38$ per FP.
- **Slides 27–32:** Halstead Software Science Metrics:
  - Basic parameters: $n_1$ (unique operators), $n_2$ (unique operands), $N_1$ (total operators), $N_2$ (total operands).
  - Program Vocabulary: $n = n_1 + n_2$. Program Length: $N = N_1 + N_2$.
  - Calculated Length: $\hat{N} = n_1 \log_2 n_1 + n_2 \log_2 n_2$. Volume: $V = N \log_2 n$.
  - Difficulty: $D = (n_1 / 2) \times (N_2 / n_2)$. Effort: $E = D \times V$. Time: $T = E / 18$ seconds.
- **Slide 33:** Knot Count Metric:
  - Formal definition: Intersection of control transfer arrows. Jump $(a, b)$ and $(p, q)$ create a knot if arrows cross. Indicator of spaghetti code.

---

### 🧪 Unit 6: Software Testing & Quality Assurance (53 Slides)
- **Slides 2–4:** Quality Definition: "Fit for use and purpose" (Joseph Juran); meeting stakeholder expectations.
- **Slides 5–6:** Levels of Testing: Unit Testing, Integration Testing, System Testing, Acceptance Testing.
- **Slides 7–12:** Testing Approaches: Manual vs. Automation Testing; White-Box vs. Black-Box vs. Grey-Box Testing.
- **Slides 13–26:** Test Plan (**IEEE 829 Standard**): 8 Steps: Analyze product, Design strategy, Define scope, Test logistics, Objectives, Test criteria (Entry, Suspension, Exit), Resource planning, Environment, Schedule & Estimation.
- **Slides 27–29:** Test Case Design & Execution Process.
- **Slides 30–31:** **Boundary Value Analysis (BVA):**
  - Testing at extremes: $Min-1, Min, Min+1, Max-1, Max, Max+1$, and Nominal.
  - **Slide 31 Example:** Input range $[18, 30]$: Test values are 17, 18, 19, 24, 29, 30, 31.
- **Slides 32–35:** Pairwise Testing (All-Pairs Testing):
  - Combinatorial testing using orthogonal arrays.
  - Slide Example: 10-item list box + checkbox (2 states) + radio button (2 states) reduces exhaustive $> 4000$ combinations down to a minimal set.
- **Slides 36–37:** State-Based Testing: State Transition Diagrams, States, Transitions, Events, Actions, State Tables.
- **Slides 38–39:** SQA Concepts: Quality Control (QC - Detection) vs. Quality Assurance (QA - Prevention). Cost of Quality.
- **Slides 40–44:** **McCall's Quality Factors (11 Factors across 3 Perspectives):**
  - *Product Operation:* Correctness, Reliability, Efficiency, Integrity, Usability.
  - *Product Revision:* Maintainability, Flexibility, Testability.
  - *Product Transition:* Portability, Reusability, Interoperability.
- **Slides 45–47:** Approaches to SQA: Preventive vs Corrective; Static analysis, Formal technical reviews.
- **Slides 48–52:** Quality Standards (ISO 9000 & 9001):
  - ISO 9000 vocabulary & principles; ISO 9001 Quality Management System (QMS) requirements.
  - 7-Step Certification Process: Application, Pre-assessment, Stage 1 Audit, Stage 2 Audit, Corrective action, Award, Surveillance. Document control requirements.

---

### 🛠️ Unit 7: CASE Tools & System Dependability (11 Slides)
- **Slides 2–4:** Computer-Aided Software Engineering (CASE) Tools:
  - Definition: Automated software tools supporting development and maintenance.
  - Central Repository: Central storage for requirements, design models, code, test cases, and metadata.
- **Slide 5:** SCRUM & CASE Tools Integration: Sprint planning, user stories tracking, sprint backlog, burndown charts.
- **Slides 6–8:** Types of CASE Tools & Benefits:
  - Upper CASE (Planning, Analysis, Design).
  - Lower CASE (Implementation, Testing, Maintenance).
  - Integrated CASE (I-CASE - Full SDLC).
  - Benefits: Cost reduction, automation, consistency, documentation quality.
- **Slides 9–10:** System Dependability & Reliability Engineering:
  - Dependability dimensions: Availability, Reliability, Safety, Security, Resilience.
  - Software Reliability Engineering (SRE) Metrics:
    - $MTTF$: Mean Time To Failure
    - $MTTR$: Mean Time To Repair
    - $MTBF$: Mean Time Between Failures ($MTBF = MTTF + MTTR$)
    - Availability: $A = \frac{MTTF}{MTTF + MTTR} = \frac{MTTF}{MTBF}$
    - Failure Rate: $\lambda = \frac{1}{MTTF}$
  - Safety Engineering: Hazard analysis, fail-safe systems.
  - Security Engineering: Confidentiality, Integrity, Availability (CIA Triad).
  - Resilience Engineering: Ability to absorb, adapt to, and recover from operational stress.

---

### 🚀 Unit 8: Advanced Software Engineering (12 Slides)
- **Slides 2–5:** Software Reuse:
  - Benefits: Increased dependability, reduced risk, effective use of specialists, standards compliance, accelerated development.
  - Problems/Inhibitors: Maintenance costs, lack of tool support, "Not Invented Here" syndrome, library search costs, architectural mismatch.
  - Levels of Reuse: Application system reuse, Component reuse, Object/function library reuse, Concept/pattern reuse.
- **Slides 6–8:** **Component-Based Software Engineering (CBSE):**
  - Definition: Development by composing pre-existing software components.
  - Component Concept: Independent executable entity with contracts (Provides Interface vs. Requires Interface).
  - **CBSE Framework Activities (Q-A-C-E):**
    1. *Component Qualification:* Evaluating fit and certification.
    2. *Component Adaptation:* Wrapping and bridging interface mismatches.
    3. *Component Composition:* Integrating components into architecture.
    4. *Component Evolution:* Updating and replacing components over time.
- **Slides 9–11:** Advanced Architectures & Disciplines:
  - *Distributed Software Engineering:* Client-server architectures (2-tier, 3-tier, N-tier), Peer-to-Peer (P2P), cloud systems.
  - *Service-Oriented Software Engineering (SOSE):* Service-Oriented Architecture (SOA), Web Services, RESTful APIs vs. SOAP, Microservices.
  - *Real-Time Software Engineering:* Systems with hard deadlines (catastrophic failure if late) vs. soft deadlines; Stimulus-response architectural patterns; Periodic and aperiodic task scheduling.
  - *Systems Engineering:* Broader context integrating software, hardware, people, and organizational processes (System of Systems).
