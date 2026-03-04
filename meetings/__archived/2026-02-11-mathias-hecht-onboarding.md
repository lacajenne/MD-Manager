Discussion with Mathias Hecht. Most of the work is around the configuration of SimCorp Dimension.
SCD dominates the configuration management. As long as SCD can only crawl, the rest cannot take off. 
We are not at a very high maturity level regarding the understanding of standardization, automation and so on.
We are not all sharing the SC1 agenda. Different stakeholders have different goals. 
The priorities are not assinged in harmony.

Client level work must take advantage of the work in the standard layer. We need to remove duplication, repetition and so on.

There are a lot of people problems, communication problems that are not technological in nature. Not every problem can be solved with technology.
Support of multiple versions is not a technological problem.

A lot of people tend to use the customer environments because the standard environment is not yet as easy to use as it should be.

70 people work in the standard environment.

Platform is providing the tools that Swiss Knives use in their work. Swiss Knives are not supposed to write tooling code. 

We could set clear milestones in testing work of the Swiss Knives. There are technical blockers. 
There is a part of the system that must be alive and functional in SC1TEST but is in conflict with configuration management. 
When it is running, the configuration cannot be modified. 

We need to start shipping full SimCorp One deliveries. 
The focus is still very much on fast delivery to single customers - sometimes at the expenses of testing. 

For the Swiss Knives - the testing part - what can wer focus on
- we still have failing pipeline running SC1DEV - we want to make it green - we are fighting structural problems - it is not a code problem
- start taking in requirements from the outcome teams (the stakeholders) - improve the collaboration in general
- we need find a way to run tests in SC1TEST - not possible now because of the conflict
- transfer some of the stakeholder specific tests into the standard environment - responsibility to fix them would stay with the original owners
    - the idea is to make them run in a better place

The stakeholders are reaching out to the Swiss Knives - who cannot really respond because they are deep in the fire brigade mode.
There is also the problem of how to make the outcome of the tests public. 
We want more interaction with the stakeholders.

PD Product Areas are being onboarded on SC1. We would like to onboard some of their tests, next to our standard ones. 
Run them with an as-is-migration. 