# SC1 Testing Strategy — Meeting Summary
**Date:** 2026-02-19  
**Attendees (mentioned):** Giuseppe, Ryan, Paul, Anette, Aleksandra, Driss

---

## Overview
Giuseppe presented a vision and guiding principles for the SC1 Value Stream testing strategy. The team aligned on evolving the approach through continuous improvement, clarifying roles and responsibilities, and strengthening data, automation, and reporting foundations across **SC1DEV**, **SC1TEST**, and client environments.

---

## Key Takeaways
- **Ownership and Accountability**
  - Value Streams own the quality of configurations and client delivery across environments.
  - SMBS and end clients are accountable for UAT; handovers should occur only once the platform is fully functional.

- **Scope and Standardization**
  - Prioritize testing in the standard SC1 environment; reserve client environments for critical, customer-specific scenarios only.
  - Rationalize tests to avoid redundancy and ensure clarity on what has already been covered.

- **End-to-End (E2E) Client Experience**
  - E2E tests are necessary to validate real customer workflows despite their complexity and cost.
  - Clear visibility is required to prevent duplicate testing across teams.

- **Quality Gates for Deliverables**
  - Deliverables (XMGR packages) move from **SC1DEV → SC1TEST → client environments**.
  - Delivery Owners should control quality gates to prevent unvalidated configurations from reaching clients.

- **Collaboration on vNext**
  - vNext is tested in PD and integrated into SC1 only after release and version alignment.
  - Support PD to achieve holistic testing prior to release.

- **Test Automation Strategy**
  - Automate where feasible and valuable; avoid automating everything indiscriminately.
  - Client environments currently rely on manual testing due to data constraints.

- **Roles and Responsibilities**
  - Outcomes configurators and Swiss Knives collaborate on test requirements, manual and automated tests in SC1DEV, and enable execution in SC1TEST; both support verification in client environments.

- **Data, Reporting, and Transparency**
  - Strategic test data management is essential: define data needs alongside configuration and test design.
  - Improve reporting and visibility to show what was tested, where, and by whom; establish clear escalation paths.

- **INTECH Pilot and Test Migration**
  - INTECH serves as a pilot to apply the new testing strategy and migrate tests into the SC1 framework.
  - Automated tests must be repeatable, independent, and manage their own data.

---

## Decisions and Principles
- Treat the current strategy as a living document that will evolve with new insights.
- Limit customer-environment testing to critical deltas, leveraging confidence built in SC1.
- Implement delivery-owner–controlled quality gates before promoting to client environments.

---

## Risks and Open Concerns
- **Test Data Constraints**
  - Difficulty supplying expected inputs/outputs without polluting client environments; this currently limits automation outside SC1.
  - Ryan raised data concerns that need explicit follow-up and resolution.

- **Coordination and Duplication**
  - Without unified reporting and handovers, teams risk redundant testing and unclear ownership.

- **E2E Complexity**
  - E2E testing is necessary but resource-intensive; careful selection and maintenance are required.

---

## Clarifications from Driss
- **Test Data**
  - The Data Team is working to provide representative test data usable in both SC1 and client environments, collaborating with requestors for validation.

- **Reporting and Transparency**
  - A first release of automated test reporting (covering SC1 runs) is approaching, enabling broader transparency on executions.

- **Automation in Client Environments**
  - Automated tests require controlled inputs/outputs; using client data jeopardizes test independence. Feasibility depends on maturity, readiness, and test data capabilities and is under investigation.

---

## Action Items
- **Test Data Management Strategy**
  - Define and implement a smarter, reusable approach to test data across environments; specify data needs alongside test and configuration design.  
  *Owner(s): Ryan, Giuseppe*

- **Testing Strategy Alignment Across Teams**
  - Publish a unified strategy that covers onboarding, upgrades, and client lifecycle testing, including what’s tested, what can be rerun, and the phase-specific deltas.  
  *Owner(s): Anette, Giuseppe*

- **Test Management, Reporting, and Escalation**
  - Establish processes and tooling for tracking coverage, environment, ownership, and clear escalation paths.  
  *Owner(s): Giuseppe*

- **Onboarding and Training (C# Test Framework)**
  - Include guidance on contributing to the C#-based framework in early-March onboarding sessions.  
  *Owner(s): Aleksandra, Ryan*

- **Address Data Concerns Raised by Ryan**
  - Consolidate issues, define acceptance criteria for “representative” test data per use case, and align with the Data Team on delivery timeline.  
  *Owner(s): Giuseppe, Ryan*

---

## Notes Integrated from Attendees
- **SMBS UAT:** SMBS should be accountable for UAT, with clear visibility into what’s already tested to avoid repetitions.
- **Collaboration with vNext:** Enable and support PD/vNext to test their configurations early and holistically.
- **Data Management Importance:** Ensure representative test data in customer environments; coordinate with data migration and governance initiatives.