# 📖 Comprehensive Software Engineering Glossary (A to Z)

[![Format](https://img.shields.io/badge/Glossary-A%20to%20Z-blue.svg)](#)

---

### A
- **Abstraction:** The software design process of hiding low-level implementation details and exposing only the essential characteristics to reduce complexity.
- **Adaptive Maintenance:** Modifying software to adapt to changes in its external operational environment (e.g., new operating system, hardware, or database).
- **Agile Methodology:** A software development philosophy based on iterative development, frequent inspection, rapid adaptation, and customer collaboration.
- **Alpha Testing:** Acceptance testing conducted at the developer's site by end users in a controlled environment with developers present.
- **Architecture Tradeoff Analysis Method (ATAM):** A formal scenario-based evaluation method developed by the SEI to assess software architectures against quality attributes.
- **Availability ($A$):** The probability that a software system is operational and accessible at a given point in time: $A = \frac{MTTF}{MTTF + MTTR}$.

### B
- **Barry Boehm's Law:** Verification is *"Building the product right"*; Validation is *"Building the right product"*.
- **Beta Testing:** Acceptance testing conducted at customer sites in real-world, uncontrolled operating environments without developers present.
- **Black-Box Testing:** Testing methodology that evaluates software functionality without knowledge of internal code logic or data structures.
- **Boundary Value Analysis (BVA):** A black-box test design technique selecting test cases at the extreme boundaries of input classes ($Min-1, Min, Min+1$, etc.).

### C
- **CASE Tools:** Computer-Aided Software Engineering tools providing automated support across the SDLC.
- **CMMI (Capability Maturity Model Integration):** A 5-level process improvement framework: Initial, Managed, Defined, Quantitatively Managed, Optimizing.
- **Cohesion:** A metric of the internal functional strength and relatedness of elements within a single software module. (Highest: Functional; Lowest: Coincidental).
- **Common Coupling:** Coupling where two or more modules share access to the same global data area.
- **Component-Based Software Engineering (CBSE):** A reuse-based approach focusing on defining, implementing, and composing loose independent components.
- **Content Coupling:** The worst form of coupling where one module directly modifies the internal code or private data of another module.
- **Corrective Maintenance:** Diagnosing and fixing latent residual bugs discovered by users during operational deployment.
- **Coupling:** A metric of the degree of interdependence and communication between distinct software modules. (Lowest: No direct / Data; Highest: Content).
- **Cyclomatic Complexity ($V(G)$):** A structural metric measuring the number of linearly independent paths through program source code: $V(G) = E - N + 2P$.

### D
- **Data Flow Diagram (DFD):** A graphical model depicting the transformation and movement of data through software processes and data stores.
- **Data Coupling:** The best form of coupling where modules communicate purely by passing simple primitive scalar parameters.
- **DRY Principle:** "Don't Repeat Yourself" — every distinct concept or business logic must have a single authoritative representation.

### E
- **Entity-Relationship Diagram (ERD):** A conceptual data model developed by Peter Chen (1976) depicting entities, attributes, and relationships.
- **Equivalence Class Partitioning (ECP):** A black-box testing technique dividing input data into valid and invalid classes where members are assumed to behave identically.
- **Extreme Programming (XP):** An agile software methodology emphasizing pair programming, test-driven development, continuous integration, and frequent releases.

### F
- **Fagan Inspection:** A formal 6-stage code inspection process (Planning, Overview, Preparation, Inspection, Rework, Follow-up) led by a trained Moderator.
- **Feasibility Study:** An early assessment evaluating Technical, Operational, and Economic viability before project sanction.
- **Functional Cohesion:** The highest and best form of cohesion where every instruction inside a module contributes to a single, well-defined function.
- **Function Point Analysis (FPA):** An algorithmic method (Albrecht) estimating software size from user functional requirements independent of programming language.

### H
- **Halstead Software Science:** A quantitative theory measuring software volume, complexity, effort, and programming time based on operator and operand token counts.
- **Hard Real-Time System:** A real-time system where missing a timing deadline leads to catastrophic system failure and potential loss of human life.

### I
- **IEEE 829 Standard:** The international standard for software test documentation (Test Plans, Test Case Specifications, Test Summary Reports).
- **IEEE 830 Standard:** The international recommended practice for Software Requirements Specifications (SRS).
- **Information Hiding:** David Parnas's design principle stating that internal module details must be hidden from modules that have no need to know them.
- **Integration Testing:** Testing phase where software modules are combined and tested to evaluate data exchange and interface communication.

### K
- **KISS Principle:** "Keep It Simple, Stupid" — software design should prioritize simplicity over unnecessary architectural abstraction.
- **Knot Count:** A structural metric counting the formal intersections of control transfer jumps in a program.

### M
- **Management Spectrum:** The 4 P's of software management: People, Product, Process, and Project.
- **McCall's Quality Model:** A hierarchical framework organizing 11 software quality factors into Product Operation, Product Revision, and Product Transition.
- **Mean Time To Failure ($MTTF$):** Average operational uptime of software before a breakdown occurs.
- **Mean Time To Repair ($MTTR$):** Average time taken to diagnose, repair, and restore a failed software service.
- **Mean Time Between Failures ($MTBF$):** Total cycle time between consecutive failures: $MTBF = MTTF + MTTR$.
- **Modularity:** Subdividing software into named, addressable components integrated to satisfy problem requirements.

### P
- **Pairwise Testing:** Combinatorial testing technique using orthogonal arrays to test all pairs of input variables, eliminating the need for exhaustive testing.
- **Perfective Maintenance:** Enhancing software by adding user-requested features or optimizing performance (~50% of maintenance effort).
- **Preventive Maintenance:** Modifying software to improve future maintainability and prevent errors (e.g., code refactoring).
- **Provides Interface:** In CBSE, the interface contract defining the services a component provides to other components (represented by a lollipop `---O`).

### R
- **RAD Model:** Rapid Application Development — an incremental process model emphasizing 60–90 day delivery cycles using component assembly.
- **Refactoring:** Restructuring internal software design without altering external observable behavior to improve quality and maintainability.
- **Regression Testing:** Re-executing existing test suites after software modification to confirm no new bugs were introduced into working code.
- **Requires Interface:** In CBSE, the interface contract defining the services a component demands from its environment (represented by a socket `---(`).
- **Risk Exposure ($RE$):** Quantified risk value: $RE = \text{Probability} \times \text{Impact}$.
- **RMMM Plan:** Risk Mitigation, Monitoring, and Management plan.

### S
- **Scrum:** An agile framework utilizing cross-functional teams, fixed-length sprints, backlogs, and ceremonies (Planning, Stand-up, Review, Retrospective).
- **Software Crisis:** The historic dilemma of software projects running over budget, missing deadlines, suffering unreliability, and becoming unmaintainable.
- **Software Engineering:** The systematic, disciplined, quantifiable application of engineering principles to software development, operation, and maintenance.
- **SOLID Principles:** Single Responsibility, Open/Closed, Liskov Substitution, Interface Segregation, Dependency Inversion.
- **Spiral Model:** Barry Boehm's iterative, risk-driven SDLC model organized into 4 quadrants: Planning, Risk Analysis, Engineering, and Evaluation.
- **SRS:** Software Requirements Specification — formal document specifying functional and non-functional requirements conforming to IEEE 830.
- **Stub:** A temporary dummy routine simulating called lower-level modules in Top-Down integration testing.

### T
- **Test Driver:** A temporary test harness script that calls the module under test in Bottom-Up integration testing.

### U
- **UML:** Unified Modeling Language — standardized visual modeling language for software architecture, containing Structural and Behavioral diagrams.
- **Unit Testing:** Testing isolated code components (functions, classes) in development isolation.

### V
- **V-Model:** A sequential SDLC model visually demonstrating the direct relationship between early specification/design phases and subsequent testing phases.

### W
- **W5HH Principle:** Barry Boehm's 7 fundamental management questions: Why, What, When, Who, Where, How, and How Much.
- **Waterfall Model:** Winston Royce's classic linear-sequential SDLC model.
