# Meeting Summary — Swiss Knives Team
Date: 2026-02-19 (UTC)

## Participants
- Kasper
- Mathias Hecht Alexander
- Giuseppe Lacagnina

## Stakeholders Referenced
- Tina (prioritization)
- Paul (strategic alignment)

## Overview
- The Swiss Knives team provides cross-cutting support for configurators and project teams across configuration management, environment handling, test automation, integration enablement, and process design. The team emerged after a reorganization to address needs that do not fit neatly into “configurator” or “tester” roles.

## Highlights by Area

### Configuration Management and Environments
- Define standards, implement them, and support configurators in moving configurations across environments with versioning and troubleshooting.
- Each configurator has access to a dev environment (e.g., SRO dev) on VMs via Citrix; multiple environments exist for different purposes.
- Managing multiple SimCorp Dimension versions is a recurring challenge; the long-term vision is an “Evergreen” model with all clients on the latest version.
- Processes adapt as new issues arise (onboarding new teams, closing legacy environments, regulatory needs).

### Test Automation
- The framework is extended incrementally (database support, API integrations) with refactoring for maintainability.
- Automated tests run in Azure DevOps pipelines (e.g., targeting SC1 test) to inject data, run batches, and extract results; failures are investigated in the pipeline UI.
- Stability and reliability are prioritized over speed; potential future levers include parallel environments and expanded mocks.
- Mocks are used for resilience and speed where appropriate, while critical flows validate against real services.

### External Integrations
- Typical flow: trades in SimCorp Dimension are sent to services like Triana for matching/reconciliation, then results are returned for downstream processing.
- The team handles technical enablement (firewalls, certificates, protocols) so configurators can focus on business logic.
- Testing blends vendor simulators, dual test accounts, and manual steps as needed, with plans to automate more scenarios and strengthen mocks for static integrations.
- Organizationally, SimCorp increasingly delivers directly to internal stakeholders, heightening the need for Swiss Knives’ technical support in workshops.

### Prioritization and Stakeholder Alignment
- Work often starts as problems/questions; the team shapes them into actionable tasks and prioritizes by impact and urgency.
- Tina leads prioritization in collaboration with the team and stakeholders; client projects influence priorities but the broader Evergreen vision guides decisions.
- Solutions are embedded into processes and ambassador groups to reduce reliance on individual heroics over time.

### Data Management and Standards
- The standard solution includes both configuration and controlled reference data (e.g., party information) to support consistency and smoother integrations.

### Onboarding and Documentation
- Daily task examples and process documentation increase transparency into workload and context switching.

## Key Takeaways
- The Swiss Knives team is a cross-functional enabler focused on stability, standardization, and practical problem-solving across environments, integrations, and test automation.
- Evergreen remains the strategic direction to reduce version drift and configuration risks across clients.
- Test automation emphasizes reliability first; mocks are leveraged selectively, with critical paths validated against real integrations.
- Prioritization is collaborative: Tina coordinates inputs from the team and stakeholders, balancing immediate client needs with long-term goals.
- Standardized configuration plus controlled reference data improves consistency and accelerates client onboarding and integration.

## Action Items
- Send the presentation discussed in the meeting to Giuseppe.
  - Owner: Kasper
  - Status: Pending