
Alignment with Driss on the Testing Strategy message for Copenhagen

- Value Stream only tests the standard configuration
- testers-configurators collaborate in the SC1 environment  
- we are building as VS a standard configuration - responsible for it e2e - we take responsibility - no there yet, this is a goal 
- value stream test leads should take responsibility to test the standard on all environments, standard and custom
- we need to automate as much as possible for obvious reasons - still needs to be stressed - know that we cannot automate everything but start with key flows
    - in collaboration with configurators and value teams
- we want an ongoing running of tests 
- example - fixed income - buy bonds - use the same data and configurations - we have an expected outcome 
- automation allows test leads to focus on improvement and extension of the test base - rather than focusing on menial tasks coming from manual executions
- automation saves resources - and lets you focus on more important things
- testing on a client environment and onboarding the client - client parametrization and client environment 
    - regression tests for client in production - we have continuous testing (compare runs in prod and test) 
    - this is partly automated 
- ideally we want pipelines in the client environments - we need data to be able to do this 
- synthetic data used in the SC1 test is close to real customer data - we sanitize client data and reuse it - tests in SC1 become very close to what clients do
- in client environments (dev and test, not prod) we need to use client data and configuration - we have idea, Thomas Olsen is involved
    - "data starter pack" idea - a set of data that can allows the client to verify complete flows - standard - same for all - usable in E2E tests
- having data usable in automated tests in the client environments makes it possible to run pipelines 
- how do we optimize testing in the client environment - drift detection report shows what changed in the standard configuration - this might help restrict the focus
    based on what was actually changed 
- testing cannot happen for client environments if we do not have a clearly defined scope - what kind of flows they will have 
    - you cannot have a test plan without a clear scope - we cannot onboard clients without a test plan - we need a clear scope from the start 
- value streams take care of testing the standard configuration and the parametrization in the custom environments 
- the ADC (Advanced Delivery Center) should test the custom client configuration - we are defining the scope of this 
- USE THE MIRO BOARD - IT JUST MISSES THE ADC PART
- UAT environment testing is done by the client and/or by SMBS  
- we are working closely with the data team to define what is needed to test as close as possible to the client workflows - data enables automated testing in the client environment 
- Swiss Knives are onboarding teams - such as Front Office - to the testing framework letting them contribute to it - we are sharing the ownership of the testing framework
    - to make it evolve faster with everyone's contribution 


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




