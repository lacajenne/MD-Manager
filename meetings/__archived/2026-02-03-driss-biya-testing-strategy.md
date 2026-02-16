
we are getting closer to a stable environment

standards are currently being defined

we do not test services, we test configurations - this is why we do E2E 

we are validating the standard configuration

configuration at this level does not cover integration (connection strings, passwords...) but of course depends on it

it is very difficult to figure out that a configuration was changed in a breaking way

configuration changes can influence each other in unexpected ways

all tests are defined to run on the same configurations

we have a dev and a test environment - the dev cannot be expected to be stable 
	the test environment needs to be stable and to be a quality gate running on a daily basis 
		the test environment needs to act as an effective gate
		
scope of the testing strategy should not be limited to the swiss knives but to all the teams working on the testing of simcorp one

we want to automate 100%

we are going to create a document together and present it to the stakeholders

the test strategy also defines how the tests are defined, written...
	sit with configurators and testers and figure out how to create tests
		how to correctly test the business flows



