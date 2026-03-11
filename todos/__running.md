
[2026-03-11]

admin work
support on Gain issue in SC1TEST
testing strategy

=====================================================================================================================================================

[2026-03-10]

Driss - question from Ryan - "test plan in ADO for intech/LT - what's the approach?"
Ola is doing it - she still needs to figure out the scope of the testing - putting it in ADO
Varun is already involved into this - they are discussing it and Varun represents Front Office 


Meeting with Roger Krishnaswamy and John Cunningham - info from Driss
There is pressure to close SP and they are under pressure for SK to enable them
	there is an issue with the current capacity
		Driss wants to allocate Mykola to build a pipeline for them 


Chat with Annalisa Abbruzzi
in Milano in SimCorp since 2003 - experience on Sophia
works on Care - customer care for Dimension
they are the contact point for customers
they do not report directly to Anette or the Value Streams - there is some suffering here
SimCorp Italiana seems to be quite separated from SimCorp - there is little possibility to commit to the Value Streams
the italian management does not share the new views and culture
she thinks people like Thomas Olsen are not thinking on the long time consequences of their choices 
	are we shortening the onboarding time at the expense of quality in production?
Value Streams are not so much a reality for her - inclusion and knowledge transfer are missing
Evergreen worries her - are we selling something we do not know we can guarantee?
Testing Services is outside of the Value Streams !!! 


Kasper evaluation of Platform is quite negative
he sees them as not agile at all - and not mature - they are afraid of letting other people do things the right way
they commit but do not deliver - this apparently happened time and again
they want to keep exclusive of the tool development - but nothing really happens 
they are going to fail


People involved in the "security structure" renaming
Matthias Stute,
Ogie Gimao,
Arjen Brokhus,
Tina W. (driver)
Natalia V. (driver)

	Matthias Stute - use him for overall intro to technical details. He also did a DEX for some analysis - maybe he ran Ogies ComSrv scripts?
	Ogie - ComSrv expert - wrote a script to analyze protected files (most likely a string search)
	Arjen - Overall solution architect for new setup. He will be able to tell us which areas are most important (FORMULAS, DEX, DFS).
 

Other topics with Aleksandra
notes emerging during the standup
 
the team reports resistance to collaboration on execution of tests, which is different from smooth operation of apps and is instead based on collaboration
it is like the configurators expect to just pass over the tests to SKs and not to have to do anything anymore - the old waterfall approach they are used to 
I see a difference in these two themes
the smooth running of apps should be based on a clear ownership
the smooth execution of tests should be based on a close collaboration between configurators and testers (SKs) 
let us review when you can
 
Another topic: the security structure large renaming task - driven by Tina and Natalia - we are having a "Saving private Ryan" moment - drop all you are doing right now and do this - Mathias and I are assigning Stefan and Dima to this 
We should discuss this as well. I am being involved in the dailies
It seems that the SKs were told not to do anything at first ("back off, this is a Platform thing") but asked later to help. Mathias seems to see this as an opportunity for the team to shine and get known
I would agree
 
=====================================================================================================================================================

[2026-03-09]

Iuliia Volkogon
head of services orchestration since one year 
	standard configuration management with its tools : XMGR, Kobold...
	part of release with Aleksandra Tina and Paul
	knows configuration challenges for value streams
		-- wants to see the testing strategy 
	mentioned Mia Malm Jorgensen


Driss - from Ola
DISCLAIMER:
This document was written from the perspective of a manual tester working in the IOS area and it is possible that my pov is limited or not fully accurate. I've tried to include my past experience, all the knowledge I currently have about the process and alignments and to keep in mind the direction we are heading. Whenever I overthought something or confused myself, I returned to the main purpose of this document, which I put at the top under the general remark.
Not all points may be applicable to your needs but I decided to include them anyway. Firstly, to provide broader context and secondly, because this exercise helps me organize my thoughts and hopefully our workflow. I plan to share it with my tester colleagues and OTs managers (Kateryna and Justyna) this week and request their feedback, so few parts might change. If it does, I’ll let you know.
I was not able to cover everything, so in some places I included only a header for an area that I consider relevant and want to define later.
Whenever I felt the need to clarify or comment on something, I added that part in italics. 
I hope you find it useful. Please feel free to comment or ask questions. I promise to prioritize any follow‑ups.



Matthias and Kasper apparently reached out to Farah - we should not reach out before talking to Kasper first - we still need the discussion 


resubmit CW request - but first a new position must be available
Mail from Farah - discuss with Aleksandra
Prepare for corporate bonus discussion with Driss - 2287.67

=====================================================================================================================================================

[2026-03-06]

Driss 
Regarding security structure, Natalia is very involved in that, so maybe reach out to her.
I am having 1:1 with ola on weekly basis, just to provide her support needed as I know she is overwhelmed, but feel free to reach out to her if you want.
regarding Iryna, we definitely need to align on what she does and what are her expectations 
Philip has some crazy idea provided from Ryan regarding the Data feed ( they are even considering taking client data and run it through AI for clean up  )  
	lets take whatever they come with a grain of salt. I also believe we are heading the right way regarding data
as for SC1TEST I need to know what his concerns are 


Value Streams page in SharePoint - Viva engage channel 

Communicate with the people mentioned for a bonus (make sure Kateryna does the same with Mykola)
Chhitiz, Driss, Stefan
	- they will get a corporate bonus
	- 80% is the achievement - give the exact amount 
	- check email from Joanna for the communication guidelines
	-- deadline 20th of march - before salaries are paid out

=====================================================================================================================================================

[2026-03-05]

Question for Driss
One question for later or whenever you have some time. I had a chat with Tomasz Pastuska and I would like to get a picture of where the Swiss Knives stand in relation to the testing for Trade Capture and Accounting. If my memory serves me, there is already some testing in place, at least for Trade Capture. Do we have any action items planned regarding this? Anything I should know or tell him?

A - we are heavy in trade capture and we started exploring front office recently - two scenarios done - will be added to the pipeline - simple happy flow - there is currently nothing in front office
	- there is no front office to go to get scenarios - Varun ignored a direct request from Driss  (can you help us find a way to test FX - he said OK - nothing after a few days)


Driss One on one
he wants to do more and keep growing and getting involved - he wants to take over work from Mathias
regarding the exit of cVation he says that we need a timeline and dates if we want things to move at all 
we need to gradually involve more and more internal people in the activities currently covered by cVation (the non-testing part)
we need a strategy for the transition
Ola Rokitka - we want to help her - she is overwhelmed - we want to include her into the testing strategy - her actual job does not match the formal description


Tomasz Pastuska
they have a lot of unit-like tests or variation on e2e scenarios - how do their tests fit in the SK schedule for SC1?
there is a lack of tests for the Front Office - Varun supposed to help there? 
he also mentioned Robert Viding
IMPORTANT: check with Driss on the trade capture and accounting tests - is my understanding correct that there is some coverage?
	- is there any action that needs to be taken here? give feedback to Tomasz

Service Orchestration team vs. Swiss Knives - what is the division of responsibilities and tasks


SK scaling
For Tina: Paul said that Swiss Knives scaling needs to be correlated with incoming clients - revenue - this is an explicit request


MESSAGE FROM DMYTRO
So about that pending updates migration into SC1TEST that I'm waiting to happen,
 
The updates were made for the Dealer Futures Trade Capture DFS "TP_TC_DEALER_FUTURE". One in particular that is of high importance for me is the removal of the formula for the Collateral Pool initialization "TP_TC_FUT_COLL".
 
I would like to know the deadline for that update. If it's not expected any time soon, then I guess I'll do it by myself. I have also asked for explicit confirmation if such update is a part of the Standard and didn't get a clear response. I'd appreciate if you can help me to confirm if that's the case.
 
I've contacted Emil Goldschneider first and later was redirected to William Bona and with his advices ended up writing to William Ekra. Getting any updates from him is especially difficult. That might be due to the fact that he is responsible for too many things and being spammed with the messages from many sides, myself included. 

MY MESSAGE
Hi William,
I hope you’re doing well. My name is Giuseppe Lacagnina, and I am the new manager of the Swiss Knives.

I am reaching out to you to support Dmytro Pavlenko. The issue is the following.
The updates were made for the Dealer Futures Trade Capture DFS "TP_TC_DEALER_FUTURE". #
One in particular that is of high importance for me is the removal of the formula for the Collateral Pool initialization "TP_TC_FUT_COLL".
 
I would like to know the deadline for that update. If possible, I would also appreciate an explicit confirmation if such update is a part of the Standard. 
That would be extremely helpful. 

Thanks very much in advance, and apologies for reaching out directly without prior contact.

=====================================================================================================================================================

[2026-03-04]

Dmytro one-on-one
they need more leverage to push a sense of urgency in some cases
need someone to pay attention when something broken emerges and it is not clear what to do 


VMO daily
- admin stuff
- testing strategy - preparing a document to present in March
- getting in the flow with the SK stakeholders - Hanna, Farah...
- discussing topics with Tina
- one-on-ones with the SKs and retrospective 

- Hanna - work with me and Driss on monitoring and E2E tests
- Aleksandra - Evergreen - some other stuff I did not get
- Dawid - topics for the management meeting 
- Artur - client onboarding value streams and some other fast jara-jara
- Giuseppe
- Natalia - readiness of drop 8 for Quonium 
- Richard - 2026 Feedback initiative
- Tina - back from Mexico



to check with Tina, for now or another session - need to know more about:
	- Value Teams
	- Deliverable Owners

Scaling discussion
linking with revenue will take place later
value streams is a cost center and not profit

we need configuration management
infrastructure management - access management 
- describe what currently cVation is covering
- come up with an estimation of what we need to survive 
- if we can start hiring now there might be a transition phase -- we should plan for the next 9 to 12 months

- need to consider replacement of cvation people
- we need also to extend the scope 
- list all facts that we anticipate or know already about - like: someone will need to cover client XYZ...
- give more concrete reasons why we need more people 
- INVOLVE DRISS IN GETTING NUMBERS FOR THE SLIDE ON THE RATIOS
- CLARIFY HOW MANY PEOPLE ARE NEEDED TO REPLACE MATTEO IN THE INFRASTRUCTURE COLLABORATION WITH MACIEJ CHOJKA 
- FIGURE OUT WHAT THE RATIO IS AGAINST ON INFRASTCTURE - PEOPLE? PRODUCT? 
- FIGURE OUT WHAT THE RATIO IS AGAINST ON 3RD PARTY CONNECTIONS 
- INTERVIEW CVATION ON A ROLE TO COLVER CROSS TOPICS SUICH AS COMMSERVER, SERVICE PLATFORM...
- NEED A MEETING WITH CVATION ON THESE QUESTIONS


=====================================================================================================================================================

[2026-03-03]

- gather information from Paul about extension - until when 
	- we need a new contract from cVation
	
- cVation to continue using Workday to record time
	- we want to start differentiating between activities
		- figure out what the task families are

- Henrik: ping Bettina -- we need to check the actual status 
	- last step we are aware of: new contingent worker
		- finance busines partner: has approved
		- background check was started as far as we know - not clear whether completed
			- if done, Henrik can start today but we did not get the IT onboarding questionnaire

- talk to Tina about Outcome Teams and Deliverable Owners
	-- they are Value Teams
	- sharepoint - who is the owner of each outcome - deliverable owners
		- look for: collaboration metrics

- reach out to Tina on the scaling of the Swiss Knives 
	- she is putting team scaling in relation with revenue

=====================================================================================================================================================

[2026-02-25]

get to know more about

- current customers - is there a snapshot somewhere
	- "Access to Environments" page

- deliverable owners - any list
	- Felix used to know - ask Marcus 
	- part of outcome teams - each team has a couple of deliverables
		- how do I learn about outcome teams? 
			- there is a data outcome team
			- check with Aleksandra

=====================================================================================================================================================

[2026-02-24]

Meeting with Aleksandra and Farah Khan (Senior Director, Value Stream - Business Services Value Stream)
DMS Value Stream - manages 15 people - 2 SCD consultants doing FTs in Gain
focus on GAIN
need to figure out how to make GAIN work in SC1


- email from Kasper - figure what to do - get back to him - cVation people get invited to trainings they do not get paid for - stop this?
- new agent: meeting notes cleanup - add highlight of most significant points - generation of md file - part of AI manager assistant
- new agent: conersationalist prompt generator - part of AI manager assistant

- from Driss - Chhitiz - does he need support? - seem a bit out of focus - Driss will reach out to him - gather feedback

=====================================================================================================================================================

[2026-02-23]

AI IDEAS
AI assistant for managers
Create an agent that has CONVERSATIONS WITH ME to give me good prompts to do what I want with AI 

Use Miro to create a personal information board


- Operational Value Streams describe the actual steps that deliver value to the customer
	- try to describe them from the customers perspective - from the outside in

- Development Value Streams describe the how things are built and chained from the technical perspective

- one should always start by picturing and understanding che operational value streams
	- how can I design the dev processes if my focus is not what I am trying to achieve from the operational, value-centered perspective?

=====================================================================================================================================================

[2026-02-20]

From Artur
Information from the Value Streams teams under Thomas Olsen who reports directly to Anette
INTECH, Lindsell Train 

relevant for the testing strategy
Razvan Radu is the onboarding lead he has got to use monday.com to make stuff visible to the clients 
Monday.com is being used as a tool to show high level plan to the customers of how simcorp delivers the projects
SIT and UAT & DR are late in the process - teams might not have enough time to resolve bugs - it makes it obvious that testing might be coming as an afterthought

this brings pressure and stress to the value streams teams
testing for Lindsell Train done by Testing services and another team (SIT testing and UAT done by SMBS)

here we are talking about the customer specific part
a lot of handovers and misalignment, possible repetition
and essentially risk - multiple parties doing testing in different stages
some context might be missing to some of the parties
are we separating too much

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

=====================================================================================================================================================

[2026-02-19]

Enrolled to "Lead with impact" for April 13 and September 21 - manage and add to calendars and todo lists

=====================================================================================================================================================

[2026-02-18]

We need to have a mopre accurate picture of the competences of Varun - to support our decisions and whatever we tell Ryan.
He is clearly not sufficiently competent from the technical side.
Mykola - assess Varun on the domain knowledge - Front Office
Driss - Varun needs to be involved into the testing strategy as stakeholder.

Driss cannot see currently a way to take Varun as a concrete stakeholder for the testing strategy
	at best he can be a bridge to front office - to figure out what is to be tested 
		-- he does not have the knowledge to give a constructive feedback
		-- he is not in the position of challenging ideas and push back


=====================================================================================================================================================

[2026-02-17]


Notes to document on "SC1 Test Strategy/Approach "

#1 
-"The SMBS..." -- make it more general, with an introduction such as "other teams..."
- Mention what the responsibility entails? test collection, prioritization, implementation, maintenance... all of it

#2 
I would explain a bit better why E2E testing is the right thing to do here. Put it in clear relation with what is being tested.
Mention the fact that other types of tests are covered somewhere else.

#5
"Only start automation..." -- not clear what it means here

#6
SC1TEST is dedicated to the testing and not to the development of tests.
Test failures should be taken as indications of real issues. Relate to the desired stability of SC1TEST.
Protected environment?

Q&A
Let us rephrase it together



Feedback to Kateryna on the "missing autotests" -- investigate


Gain performance issue
Bettina and replacement for Felix




talk to Chhitiz about his leave
talk to Marcus
talk to Kasper
promotion of Driss - chat with Aleksandra and Kateryna

=====================================================================================================================================================

[2026-02-16]

[16:30]
What tasks are coming to the team? From where? Are they in the scope of SK?
Same question about Felix. Is he the only one who can do what he is doing?

[13:30]
Notes from Natalya V.

Felix is going to be replaced
	he has the knowledge to support the configurators
	in case configurator requests keep coming they should be redirected to the CDS team
	ideally he should be replaced by some simcorp internal or someone who is shadowed by a simcorp internal
	
we had apparently a bi-weekly review that was cancelled, between SK and their stakeholders
	we are expected to reiterate again, maybe on a monthly basis
	
[11:00]
From Aleksandra for Driss

Hi! I just got these messages from Aleksandra - let us discuss it when you are back 
 
 
Hi - I have this question from Tomasz Pastuszka who is one of the stakeholders from PD application areas that are moving into SC1 environments. I need us to prepare an answer to this for tomorrow afternoon:
"Dear All - I am interested in understanding where the whole Test Automation topic is now - perhaps we can discuss this next Tuesday if anyone here can provide an update? I can see teams are getting more and more serious about working in SC1DEV but the engineers/configurators are still not supported with regards to being able to run automatic tests of their work and no update was yet provided on this through general channel as far as I noticed."
this is about a topic related to movement from Standard Platform to SC1 environments. In SP, there were some automated tests running and I am pretty sure that Tina was exploring with SK the possibilities to (re)use them, but I am not sure if this was pursued further, abandoned, evolved... so we need some updates... and - we need to find a way to track these topics somehow (ideally from DevOps)

=====================================================================================================================================================

[2026-02-13]

[09:30]
- involvement with the testing strategy - and getting to know the testing framework
- Kanban related
- completing handover
- Pink Elephant work

=====================================================================================================================================================

[2026-02-12]

[14:00]
Natalia Voitsekhivska
SimCorp Dimension Academy - something to sign in to - check with Aleksandra

We do not have people for the execution of the Front Office tests.
Apparently Varun was promised to have a team. 


[10:30]
VMO Planning priorities
1- Urgent (Unplanned) - up to 2 weeks + requests from LT
2- Un-/Planned activities with deadline or high impact on other teams- up to 4 weeks
3- BAU & Planned - continuous tasks(daily/weekly/monthly activities) + planned without dependencies with middle or lower impact
4- Ideas/Plans with unsolved dependencies,but it is on our radar

Planning notes
We are going soon to onboard a lot of new people on Value Streams teams (30-50).

=====================================================================================================================================================

[2026-02-11]

[16:00]
Driss Biya and Florian Prinz

DMS Value Stream should be responsible for DM Core upgrades in the standard environment. 
26.01 upgrade for SimCorp Dimension will require DM Core to be upgraded too.
Platform people are responsible for deployments.

We want to talk to the DMS Value Stream to see how they are going to manage this in the future.
And see who else should be involved.

=====================================================================================================================================================

[2026-02-05]

[13:45]
Question for Driss.
Hi! I am starting to build a picture in my head about the work of the Swiss Knives. I’d like to get a sense of where the Swiss Knives team stands at the moment: are you already in a normal operational rhythm, or are you still dealing with a higher share of urgent or temporary tasks while moving toward that steady‑state mode?

[16:00]
Salary Review 2026 - Tobias Sheppard

- pay outcomes feel deeply personal to employees - can feel equally challenging for managers

- there are a lot of sources of pressure: fainness, budget, performance data, morale, expectations... 
    and the EU Pay Transparency requirements

- annual salary review is a check point to validate employee compensation, considering performance along with positioning
    within the pay range and against peers

- approach - data driven
- fairness principle - considering location, performance and position in the range (compa-ratio)
- communication
- practicalities 

Learn about Compa Ratio - actual salary / mid range point

High level principles
market alignment - we benchmark with the technology sector but also consider financial services for some roles
competitive positioning - total cash compensation is centered around market median to insure internal equity 
pay fo performance

[11:00]
Chat with Driss.
SimCorp One going into Value Streams.
There are people going to do front office configuration - new people involved in the whole workflow.
Joining back and middle office in value streams - front office probably are not that mature
Ryan started hiring people without being aware - or ignoring - what was aready happening.
He was looking to hire people for front office when SKs are already covering the process E2E.
He hired Varun - but it was not a good fit. A lot of confusion, a lot of time was spent onboarding him. 
There was a strict hiring process and this hiring jumped over it completely - Varun does not have any of the mandatory knowledge.
He is creating chaos and noise right and left inviting a lot of people that are not concerned - an agent of entropy.
We need to stop this noise from the outside. 
If he accepts to fully work as a Swiss Knife, the team is ready to accept him. 

[10:30]
Chat with Dmytro Pavlenko. 10 years experience, with SimCorp since November. Works in Warsaw.
Works in test automation mostly. Seems as skilled and confident as all others.
Sees cVation as Site Reliability Engineers mostly.
He finds the stress levels acceptable, the environment friendly.
They are building a network of contacts and escalation paths appear to exist.
I told him about my approach - that I will observe, that I know that the team is pretty independent already.
I do not wish to change things in a top-down approach. I want to get there together with them, sharing vision and strategy
from the company. The ceremonies we are going to implement are to be discussed within the team, and we want to reach a pragmatic agreement
on whatever workd best.

[09:45]
Varun was hired in VS SC1 as Test Architect. No one knows what he is expected to do. 
He was tasked to create a testing strategy. But there was a draft from the Swiss Knives that was approved by Paul.
Whatever happend with Varun - he has not the knowledge [Driss] - and SKs are already working on it.
We have a conflict. Discuss with Aleksandra. He came and did not find anything to do because there was already a framework 
    - he volunteered for a testing strategy.
There was apparently an issue in communication.
He should be onboarded with the team, brought to the team and let him do what he wants under the umbrella of SK.
Natalia and Driss wanted to talk with Ryan but apparently were not allowed.
Varun seems to have the wrong compentences and aspirations.

[09:30]
Continuing onboarding and testing strategy discussions
Following the topic with Driss and Florian, we have planned a meeting, going to figure out if other people need to be involved

[09:00]
unplanned work - reserving buffers for unplanned work
customer feedback - the cycle does not hand when we hand stuff over - the feedback is a new starting point

Check the SharePoint site on Value Streams

=====================================================================================================================================================

[2026-02-04]

[16:55]
Maybe we can define a timeline for these upgrades together. My understanding is that we want

to announce them at least a few days in advance
figure out how long they will take and whether we expect down time


[13:30]
A lot of topics are covered by cVation people in SK.
Swiss Knives were supposed to be temporary but have become a long term thing.
Workload keeps increasing - SKs are working to empower people - but even with this approach, SK need to grow.
The amount of stuff to be tested is also rapidly increasing and might explode suddenly.

Mathias Hecht Alexander
wave 1 - the start - 1 SK to 2 configurators
wave 2 - onboarding of value teams
wave 3 - Standard Platform - 1 SK to 10 configurators 

