# questions - open points

- describe Value Streams as organization
    - are they collections of teams...?

- need to know more about the configurations to be managed in Value Streams
    - what products
    - what format
    - run-time vs. build

- what is SC1DEV

- Client Product Environments
    - what products
    - who has access
    - who gives support
    - who is responsible for SLAs and such

- SMBS teams - what are they 

- End-2-End testing
    - what products and system components are we talking about
    - rule: minimal critical E2E journeys

- are these environments? where do they live?
    SC1DEV > SC1TEST > CLIENT ENV
    - are we shifting some tests to the left?
    - understand the flow(s)

- understand deliverables

- "all tests should be automated at some point" - needs refinement 
    - gate manual tests need to be reduced to the absolute minimum
    - left shifting is also very important
        - doing each test in the right place of the flow and at the right time

- #6  discuss 

- client environments are like staging?

- missing? reporting and analysis of test results 
    - success rates
    - flakiness
    - duration

- Q&A section
    - repeatable means that they can be repeated without changing the outcome
    - individual: order of test execution must not matter


# notes

- DEV gates: fast, cheap, stable
- TEST gates: broader, more realistic, integrated, system-level
