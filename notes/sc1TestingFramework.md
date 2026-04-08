Describe the test flow logic - setup - run - assert - waiting & syncrhonization - teardown
Elaborate on polling, explicit waits, retries, timeouts
Elaborate on the flow of test data
Is anything mocked?
Is data cleaned up? when?
Is test execution idempotent?
 
How readable are the existing scenarios?
How easy it is for a new contributor to add a new meaningful test scenario?
How hard would it be to introduce a Gherkin-like feature file layer?
Is the framework clean and ready for contribution?
 
What is needed to write test locally?
Where can tests be run?
 
What are the most relevant current limitations of the framework?
How many functional areas / test families cannot be implemented in the framework due to its incompleteness?
 
Is parallel test execution a meaningful topic in this context? Does the framework support it?
Elaborate on the risk of test flakiness and the corresponding mitigation strategy
 
When tests fail, how easy is it to figure out why?
How good are logging and reporting?
 
How well is the framework documented?
Are there guardrails that prevent misuse of components and common mistakes?
How well do framework unit tests insure that the tests are doing what is expected?
 
Extra topics:
coding guidelines
static analysis and linting