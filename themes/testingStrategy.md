
## Alignment with Driss on the Testing Strategy message for Copenhagen

**Ownership & Responsibility**
- Value Streams test the standard configuration and are responsible for it end-to-end (goal, not yet fully achieved)
- Value Stream test leads should take responsibility to test the standard on all environments — standard and customer specific
- Testers and configurators collaborate in the SC1 environment
- The ADC (Advanced Delivery Center) should test custom client configuration — scope is being defined
- Value Stream test leads test the standard configuration in client environments - we are trying to find the sweet spot between how much we can test and how much we can automate 
- UAT environment testing is done by the client and/or by SMBS

**Automation**
- Automate as much as possible, starting with key flows — in collaboration with configurators and value teams
- We cannot automate everything, but automation frees test leads to focus on improving and extending the test base rather than manual execution
- We want ongoing, continuously running tests
- Example: Fixed Income — buy bonds using the same data and configurations, with an expected outcome

**Test Data**
- Synthetic data in SC1 is close to real customer data — we sanitize client data and reuse it
- In client environments (dev and test, not prod) we need client data and configuration
- "Data starter pack" idea: a standard set of data enabling clients to verify complete flows, usable in E2E tests  — Thomas Olsen is involved
- Working closely with the data team to define what is needed to test close to real client workflows — solving the data issue enables automated testing in client environments

**Client Environment Testing**
- Ideally we want pipelines also in client environments — we need data to enable this (through test automation)
- Drift detection report shows what changed in the standard configuration — can help restrict testing focus based on actual changes - under scrutiny
- Regression tests for clients in production via continuous testing (compare runs in prod and test) — partly automated

**Scope & Planning**
- Testing cannot happen for client environments without a clearly defined scope of flows
- You cannot have a test plan without a clear scope — we cannot onboard clients without a test plan
- A clear scope is needed from the start

**Collaboration & Framework Sharing**
- Swiss Knives are onboarding teams (e.g. Front Office) to the testing framework, sharing ownership to make it evolve faster with everyone's contribution


Discussion with Artur Cybruch, 260220

-- this is all to be confirmed - not being affirmed - we are getting attention to assess a risk that impacts the testing strategy
-- we are talking about customer specific testing
-- many teams are involved with complex handovers and possibly loss of context and other inefficiences
-- it seems there is overall too much complexity in the way the work is managed across teams
-- it seems that the testing (SIT, UAT, DR) are happening LATE (shortly before go-live) and seem to be an afterthought
-- relevent customers are INTECH and Lindsell Train (SC1, therefore more relevant)
-- affected teams are Value Streams Teams responding to Thomas Olson and Ryan Glass 
-- source of this information is partially Monday.com that is shared with the customer and stakeholders to show planning 
-- testing strategy is certainly relevant here 

-- https://miro.com/app/board/uXjVJoLMS1Y=/?share_link_id=499816057435

- check out existing Value Stream Maps and clarify the current status of things
- map what needs mapping - teams, workflows and so on
- is there any low-hanging-fruit improvement that we might go for?
- value stream feedback document
    - start from the items on testing, select the most important ones
    - play the 5 whys game - incorporate into the testing strategy
- document on the ARDEA escalation
    - it mentions the need of detailed test plans 
        - we need traceability for the plans to be useful 
            - how can you validate a plan if you cannot trace it back to some requirement
- test data
- testing frameworks and tools - do we want to have more than one framework?
- reporting and evidence 
- collection of test execution data, across all tests
- health checks for the test environments?
- retro sessions on the testing process
- quality gates and risk assessment and mitigation
- feedback loops on the whole process
- scalability
- where do tests live? Plans, definitions... 
- coverage




