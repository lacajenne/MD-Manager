- Describe the test flow logic - setup - run - assert - waiting & syncrhonization 
 
    Setup
    Execute by batch job groups - this is time consuming
    Assert

    Tests are parallelized by the xUnit framework - distinct classes are run in parallel (tests inside each class run sequentially)

    Scheduled runs involve a 9 hours delay 

- Elaborate on polling, retries, timeouts
    Usually yes 

- Elaborate on the flow of test data
    We create it mainly using the FW - sometimes data is created manually in SCD and then added to the FW - the pipeline uses XMGR to update the test system with the new data

- Is anything mocked?
    No

- Is data cleaned up? when?
    At the moment we do not have it, but we plan to 

- Is test execution idempotent?
    Yes

- How readable are the existing scenarios?
    Not easy
    Some README files have been added
    It requires coding skills and business knowledge
    Not easy to fully reconstruct what the test is doing and what it is asserting - difficult to edit/fix the test

- How easy it is for a new contributor to add a new meaningful test scenario?
    It requires coding skills and business knowledge
    It requires collaboration with the configurators

- How hard would it be to introduce a Gherkin-like feature file layer?
    Apparently it was attempted and produced poor results
    We can still consider it

- Is the framework clean and ready for contribution? 
    Not yet - but we are not far away from it - we want to do some refactoring

- What is needed to write test locally?
    Follow README instructions
    Environment access
    Development tools 

- Where can tests be run?
    Tests always run in some of the cloud environments (SRODEV for development)

- What are the most relevant current limitations of the framework?
    Entities cannot be created at run time - there is no dedicated API to do so - not a strong limiting factor 
    Might be solved by Data Starter Pack 

- How many functional areas / test families cannot be implemented in the framework due to its incompleteness?
    None as far as we know - currently

- Is parallel test execution a meaningful topic in this context? Does the framework support it?
    Yes. See above

- Elaborate on the risk of test flakiness and the corresponding mitigation strategy
    The only significant source of flakiness is coming from manual interventions on the test environments

- When tests fail, how easy is it to figure out why?
    It is not easy due to the nature of the system and its flows
    When tests fail in the setup phase, it is easy to reconstruct what happened - but even in this case, not always
    In general debugging failed tests requires a significant system knowledge

- How well is the framework documented?
    README files are good enough to start

- Are there guardrails that prevent misuse of components and common mistakes?
    We are trying to do so through the architecture

- What coding guidelines are going to regulate contributions to the framework?
    TBD

- Elaborate on static analysis and linting for the framework
    We will consider adding it when there are more contributors 
