1. Configuration Management (CDMS / XMGR)
Decision-making around non‑standard transports and dependencies
Handling of protected entities, deliverables, and edge cases
Client‑specific constraints (e.g. RO access, partial deploys) and how to work around them safely
Judgement calls where rules or documentation are insufficient

2. Environment Management & Infrastructure
Understanding and managing SC1 / SRODEV / client environment lifecycles
Upgrade sequencing and readiness decisions
When environments are technically available vs. when they should not yet be used
Typical failure modes and how to diagnose them

3. Client / Project Support (complex cases)
Escalated support situations that require cross‑area understanding
Deciding when to resolve locally vs. escalate further
Patterns of recurring issues across clients/environment types

4. Access & Authorization (decision layer)
Interpreting and resolving non‑standard access situations
Understanding side effects of access packages and profiles in specific environments

5. Automation / Tooling (governance & integration)
Judgement on what should be automated vs. handled operationally
How automation, environments, and CDMS fit together in practice

6. Operational / “Glue” Responsibilities
Areas where he currently acts as a stabilizing or coordinating point across teams
Topics where ownership is implicit rather than formally defined



from Mathias himself

Hi Aleks,

Thanks for putting this together🙂

I would simplify the list into two big categories:
Overseeing (and participating in) the Swiss Knives support organization (coordinating all teams, friends and family keeping SC1 "online").
Driving (or being a primary participant in) process design, strategic initiatives, politics, and architectural decisions.

Handover notes on Swiss Knives "support".
This area is too massive to put into categories. I'm confident Felix, Marcus and Matteo will cover all bases here, and Henrik and Kasper will support when necessary, on strategy, process and politics. This also means when "support" topics are to be raised to category 2 on the list above.

Notes on process design, strategic initiatives, politics, and architectural decisions.
This is my key role. Kasper and Henrik will cover this. This is the primary topics:
SC1 Release
    Config bundle MVP across XMGR, CDMS and CMD
    Potential beta-version of deployment schedules before bundling)
Client Parameter Contribution flow
    Potential "minor version" Deliverable when doing customizations. 
"Lead" the ambassador group
Platform features (validation & feedback)
Platform alignment (requirements & prioritization)
    This is likely where my absence will leave us the most exposed. The "centralized governance of priorities" from VMO/Value Streams will help a lot. I was part of the first discussion on this topic, and I know there was some development, but we need to get it "activated", and then we will be much less exposed 🙂 Basically, the VS must own its own priorities (maybe just a public list?), centrally managed and clearly communicated to Platform.
    