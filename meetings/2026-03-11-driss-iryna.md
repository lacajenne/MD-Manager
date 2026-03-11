
## People
Driss Biya, Giuseppe Lacagnina, Iryna Vernyhora

## Purpose
The meeting focused on clarifying testing responsibilities across teams, addressing capacity and collaboration challenges, and exploring the foundations of a unified testing strategy spanning standard development through client onboarding.

---

## Key Topics & Outcomes

### 1. Clarification of Testing Responsibilities
There is ongoing confusion regarding ownership of **end-to-end (E2E) testing in client environments**, particularly for **parameterized standard configurations** versus **client-specific custom configurations**.

- **Current role confusion**:  
  It is unclear whether Value Stream test leads or ADC consultants are responsible for E2E testing in client environments, leading to overlap risks and uncertainty in capacity planning.
- **Standard vs. custom configurations**:  
  ADC testing has primarily focused on client-specific custom configurations, while Value Stream testers were assumed to handle E2E testing of parameterized standard flows. This assumption requires confirmation.
- **Capacity concerns**:  
  Unclear responsibilities risk overloading teams and causing redundant testing efforts.
- **Decision & alignment needed**:  
  Previous discussions with Annette and Thomas were referenced. Stakeholder alignment is required to confirm ownership and support upcoming project planning.

---

### 2. Development of a Unified Testing Strategy
The group discussed creating a **single, end-to-end testing strategy** covering standard build, validation, and client onboarding.

- **Strategy objectives**:  
  Align functional, E2E, automated, and continuous testing across standard and client environments; identify gaps; reduce redundancy.
- **Inclusive approach**:  
  All relevant teams, including ADC, should be involved in shaping the strategy through additional working sessions.
- **Avoiding redundancy and overload**:  
  Clear responsibility definitions and scoped test scenarios are required to prevent duplicated effort, especially as client numbers grow.
- **Document alignment**:  
  A corporate task strategy document for client-facing activities exists and should be aligned with internal testing approaches to avoid inconsistencies.

---

### 3. Collaboration Between Teams and Clients
Different collaboration models were discussed depending on whether SMBS is involved.

- **Shared environment with SMBS**:  
  A single shared testing environment is being considered, requiring coordination of schedules and activities; details are still to be validated.
- **Clients without SMBS**:  
  ADC aims to complete E2E testing before client testing starts, then support clients during execution and defect management.
- **Environment stability**:  
  Early testing in unstable client environments has proven inefficient; stable data and configuration are critical for effective testing.

---

### 4. Automation & Continuous Testing in Client Environments
The feasibility of reusing automation and extending continuous testing earlier in the lifecycle was explored.

- **Automation reuse**:  
  Reusing standard automated tests in client environments could enable sanity checks and early regression detection.
- **Technical limitations**:  
  Current pipelines generate synthetic test data and do not support client-specific data, limiting direct reuse.
- **Continuous testing scope**:  
  Continuous testing is currently production-focused; expanding it to earlier stages could reduce manual effort.
- **Incremental approach**:  
  Small-scale pilots (e.g., AXA, Intac, Lean cell) were proposed to validate feasibility before broader rollout.

---

### 5. Testing Approach: End-to-End vs. Component Testing
A balanced testing strategy was agreed as necessary.

- **End-to-end testing**:  
  High value for validating real client workflows and detecting integration issues.
- **Component testing**:  
  Useful for earlier issue detection and lower cost of fixes.
- **Conclusion**:  
  Both approaches are needed, with clear guidance on where each provides the most value.

---

## Follow-up Actions

1. **Clarify testing ownership**  
   Confirm and communicate which team owns E2E testing for parameterized standard configurations in client environments.  
   *Owners: Driss, Iryna*

2. **Align testing strategies**  
   Share the corporate task strategy document for client-facing testing and gather feedback for alignment with internal approaches.  
   *Owner: Iryna*

3. **Evaluate automation reuse**  
   Assess feasibility of reusing automation in client environments, starting with pilots in AXA, Intac, and Lean cell.  
   *Owners: Iryna, Driss*

4. **Plan follow-up session**  
   Schedule a session to address open questions on collaboration models, environment usage, and capacity planning.  
   *Owners: Driss, Iryna*
``
