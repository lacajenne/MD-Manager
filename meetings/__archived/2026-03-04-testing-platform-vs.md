# Meeting Summary: Unified Testing Strategy and Platform Alignment

This meeting covered SimCorp’s move to a unified system integration testing strategy and framework, the platform team’s responsibilities, definitions of system integration vs. end-to-end tests, environment/tooling requirements, execution strategies, and reliability improvements. A draft value streams testing strategy is targeted for end of March, with a follow-up in early April to align roles and implementation details.

## Key Takeaways
- SimCorp will adopt a single, unified strategy and framework for system integration tests organization-wide, owned by Piotr’s platform team.
- Consultants (not developers) build tests using the provided framework and building blocks; domain experts define flows, and automation specialists add missing step implementations.
- Tests should embed prerequisites (e.g., data creation) and cleanup for repeatability and reliability.
- The testing platform is infrastructure agnostic and runs locally, on customer VDIs, in Team CT, and Azure Pipelines; TAS is available for pipeline integration.
- Flakiness is mitigated via explicit waiters, with ongoing efforts toward unified authentication and direct API communication.
- Parallel execution is conceptually supported; the current parallel agent count is hardcoded to one, with parameterization planned.
- Continuous testing already uses the platform in client repositories (coverage varies); some environments (e.g., Quanium) use separate copies to isolate testing from development.
- A testing council is being formed to define holistic approaches (onboarding, configuration, automation) and ensure cross-team alignment.

## Decisions
- Adopt a unified test strategy and framework for system integration tests across SimCorp.
- Transition Piotr’s team from testing services to platform to make the testing platform available to all stakeholders.
- Establish a testing council to drive a holistic testing approach and cross-departmental collaboration.

## Discussion Highlights
- Definitions and scope
  - System integration tests: Validate cross-system interactions (example: Synchron Dimension with satellite apps like Snowflake) within a single automated scenario.
  - End-to-end: No full examples yet; front office work in progress (e.g., SD web API portfolio sheet validations). Users can add custom step definitions as needed.
- Environment and tooling
  - Supported runs: local machines, customer VDIs, Team CT, Azure Pipelines.
  - Prerequisites on VDIs: Coordination underway with Charles Alba and the “straw hats” team to pre-install PowerShell 7.5 and .NET 8 in master images.
- Reliability and data
  - Tests include setup/teardown to manage prerequisites and cleanup.
  - Explicit waiters address variable processing times (e.g., GAIN); unified auth and direct APIs planned to further reduce flakiness.
  - Data concurrency: Prior approach uses unique values per test; shared client environments require careful handling to avoid conflicts.
- Execution strategy
  - Suites can run serially (stop on failure) or in parallel; future work will parameterize the number of parallel agents.
  - Environment hygiene remains challenging; options include dedicated/short-lived environments and local runs for initial test development.
- External integrations
  - ETM, Triana, Trioptima, Cassini not considered in early stages; potential future enhancements.

## Action Items
- Testing Platform Onboarding Communication
  - Send follow-up email to Paul and relevant stakeholders confirming agreement on the unified testing platform and outlining onboarding next steps. (Owner: Piotr)
- Testing Platform Prerequisites Installation
  - Coordinate with Charles Alba and the “straw hats” team to pre-install PowerShell 7.5 and .NET 8 in master images for customer VDIs. (Owner: Piotr)
- Testing Council Participation
  - Invite Driss to upcoming testing council calls to contribute challenges and input on the holistic testing strategy. (Owner: Piotr)
- Testing Strategy Draft Review and Follow-Up
  - Schedule a follow-up meeting in early April to review the value streams testing strategy for SimCorp One and define roles/responsibilities. (Owners: Piotr, Giuseppe, Driss)

## Timeline and Next Steps
- Draft testing strategy for value streams: end of March.
- Follow-up meeting: early April to confirm roles, responsibilities, and integration points with the testing platform.

## Participants Mentioned
- Piotr (Platform/testing platform lead)
- Driss
- Giuseppe
- Ulrike (Platform)
- Paul
- Charles Alba
- “Straw hats” team