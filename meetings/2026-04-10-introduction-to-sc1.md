
# Introduction to SC1 — Meeting Notes
*2026-04-10*

**Presenter:** Mathias Hecht Alexander
**Participants:** Raj Bahadur Singh, Anel Odobasic, Prakhar Gupta, Payam Chini Foroushan, Giuseppe Lacagnina, Kasper Fehrend, Vishal Jain

---

## Standard Deliverable Contribution and Release Workflow

Mathias led a comprehensive walkthrough of the standard deliverable contribution and release process, covering the technical steps, versioning, validation, and approval mechanisms in X Manager.

- **Development and Contribution Flow:** Configurators begin work in the SRO dev environment, performing configuration and basic verification before extracting changes into a deliverable using X Manager. The process involves selecting entities, updating package definitions, and ensuring changes are associated with the correct functional area and track. The contribution template in X Manager is used to formalize these changes, and the workflow is initiated by executing the package action.
- **Package Definitions and Versioning:** Each deliverable is tied to a package definition (metadata listing entities) and an immutable package (actual content with a hash). Every contribution creates a new package hash, ensuring immutability and traceability. Multiple contributions can be made before an official release, and only upon release does the package become available for further testing and deployment.
- **Validation and Overlap Checks:** The process includes validation to prevent entities from being included in multiple deliverables. If a user attempts to add an entity already present elsewhere, the system blocks the action and notifies the user. Overlap checks are enforced both for standard and client-specific deliverables.
- **Approval and Testing Process:** After contributions are released to the SC1 test environment, an approval workflow is triggered. Approvers (determined by access packages) must verify the deliverable through manual or automated testing before approving. The approval step is the final gate before deployment to SC1 gold and subsequently to client environments. Supports fix-forward principles — no rollbacks.
- **Handling Errors and Rollbacks:** If deployment or approval fails, a new contribution is required to address the issue, followed by another release and approval cycle. There is no automated rollback; errors must be fixed forward. The system supports exporting current states before imports for potential manual rollback.

---

## Parameterization and Custom Entity Management

Mathias, with input from Kasper Fehrend, detailed the parameterization process for client-specific customization.

- **Custom Entity Flagging:** During contribution, configurators must flag which entities are eligible for client-specific parameterization. Only flagged entities can be customized at the client level; the rest remain standard and immutable. Managed via the `flag custom entities` action in X Manager.
- **Parameterization in Client Environments:** When a deliverable is deployed to a client environment, entities marked as custom are left empty or with dummy values, allowing client-specific parameterization. Unauthorized changes are overwritten by subsequent standard deployments.
- **Sidecar Package Mechanism:** Client-specific parameter values are stored in a separate "sidecar" package travelling alongside the standard immutable package. Standard content remains unchanged while client customizations are layered on top.
- **Field-Level Granularity and Future Improvements:** Currently parameterization is managed at the entity level — all fields within an entity are marked as custom if any require customization. Field-level granularity is a recognized gap with ongoing work to address it.
- **Process for Changing Custom to Standard:** If an entity previously marked as custom is reverted to standard, the next standard deployment will overwrite any client-specific changes. No automated merge from client to standard; changes must be reintroduced via the standard contribution process.

---

## Patching and Version Compatibility Management

Mathias and Kasper described the patching process for supporting clients on older versions.

- **Patch Track Workflow:** For clients on older versions (e.g., 2510), a separate patch track exists. Patches are created by extracting entities from SC1 gold and deploying them to the appropriate versioned environment using a dedicated patch deliverable template in X Manager. Only entities from gold can be patched down.
- **Handling Backward Compatibility:** If a patch is not backward compatible, the deployment fails and the user is notified to resolve manually. No automated snapshot restoration — fix forward only.
- **Auto-Contribution and Testing After Patch:** Successful patches trigger an automatic contribution and release in the target environment, followed by a pending approval for testing.
- **Version Filtering and Transport Logic:** The transfer adapter transports all deliverable versions to client X Managers, but deployment scripts ensure only compatible versions are deployed to each environment. Filtering logic to optimize storage and deployment is under discussion.

---

## Client-Specific Deliverables and Change Management

Mathias and Kasper explained the handling of client-specific deliverables and enforcement of overlap checks.

- **Client Deliverable Workflow:** Client-specific deliverables follow the same contribution, release, and approval process as standard ones. Named distinctly (e.g., `Adea_FO`) and used for purely client-specific configuration transport.
- **Overlap Checks and Entity Ownership:** Entities cannot exist in both standard and client-specific deliverables, nor duplicated across multiple client deliverables. Any violation results in a block.

---

## Approval Roles, Access, and Process Limitations

Vishal Jain, Payam Chini Foroushan, and others discussed limitations of the approval process.

- **Approver Assignment and Access:** Approvers are determined by access packages. Currently, anyone with the package can approve any deliverable — leading to occasional unauthorized approvals. Recognized as a flaw; improvements planned to restrict approvals to appropriate owners.
- **Approval and Rejection Mechanisms:** The approval interface has both approve (green) and reject (red) buttons. If a deliverable is not approved, a new contribution and release is required. No automated revocation of previous approvals.

---

## Testing Strategy and Automation

Giuseppe Lacagnina, Payam Chini Foroushan, and Kasper Fehrend discussed the current state and plans for automated testing.

- **Current Testing Practices:** Testing is primarily manual, with some automated tests run in SC1 test using the Swiss Knives and twin test suite. No comprehensive pipeline for automated checks across deliverables.
- **Plans for Enhanced Automation:** The team is building a framework for integration tests, enabling teams to develop automated tests for their features.

---

## Auditability and Logging

*Giuseppe Lacagnina inquired; Mathias confirmed.*

- **Audit Logging Coverage:** All significant actions in the contribution, release, and approval workflow are logged — including who performed actions, when, and on which entities or deliverables. Technically comprehensive, but accessing logs may require technical effort.

---

## Dashboard Usage and Future Training

*Anel Odobasic requested more information; Mathias suggested a follow-up session.*

- **Dashboard Indicators:** Uses color indicators (green / yellow / red) to show deployment status for deliverables across environments.
- **Planned Technical Deep Dive:** A follow-up session will be organized with technical experts (David or Christoph) to cover dashboard features, tags, and backend processes. Participants should prepare specific questions in advance.

---

## Follow-up Tasks

| Action | Owner |
|--------|-------|
| Set up a technical deep-dive session with David and/or Christoph (background tooling, tag meanings) | Mathias, Anel |
| Organize a dashboard training session (deployment statuses, cross-client tracking) | Mathias |
| Share dashboard links and access with participants who requested them in the chat | Payam |
