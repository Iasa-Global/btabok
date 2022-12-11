--
title: "Advanced Quality Attributes"
keywords: 
sidebar: mydoc_sidebar
toc: true
permalink: advanced_qa.html
folder: competency_model
summary: "Requirements are not sufficient to develop architecturally good software."
tags:
  - software_architecture
--

# Description

**Q**uality **A**ttributes (QA), though a non-functional requirement, cannot be explained without functional requirements. Since differing focus on Quality Attributes lead to difference in software architecture even though the requirements remain same, it is more meaningful to call these 'non-functional' requirements as 'extra-functional' requirements.

Learner must be through various QAs and its definitions and primary applicability explained under Quality Attribute Pillar. In this the focus is mainly on

-   How to discover a QA?
-   How to choose which QA to prioritize
-   Why to de-prioritize a QA so that another QA can be prioritized? What trade-Offs?
-   How to identify a tangible cost involved in implementing a QA?
-   How to identify and list out tangible benefits of a QA? This helps in prioritizing a QA over another.
-   How to enable decision making using QA cost and benefits?

# Overview

Requirements are not sufficient to develop architecturally good software. Different architects would produce a different architecture for the same requirements. An architect who had elicited and understood Quality Attributes well can have a better architecture than the others.  Additionally, one who had understood underpinning of quality attributes with other QAs can have a much better architecture.

Architect should conduct **Q**uality **A**ttribute **W**orkshop (QAW). Architect should carefully collect **A**rchitecturally **S**ignificant **R**equirements (ASR) as an outcome of QAW. If a requirement affects the making of a critical architecture design decisions, it is by definition an ASR.

Then architect should list out tangible and intangible cost and their benefits. Use this information to prioritize few QAs. Attribute driven design will help in better software design. Architect should keep stakeholders in the loop all through the design and development process.

Architect is the primary owner of this skill. He needs to eke out information from the stakeholders. Stakeholders mostly think from requirement perspective while Architect has to think from current implementation and future extensions as well. Stakeholders' primary concern is cost while Architect's primary concern is to identify crucial QA and implement them to stakeholders' satisfaction.

Architect has to focus on requirements that are architecturally more important. For this (s)he should be able to identify ASR.  For identifying ASR (s)he is required to organize a QAW or similar effort to collect scenarios. Without clarity on these it is difficult to provide an architecture that suits the stakeholders current and some future requirements that are predictable today.

# Proven Practices

Quality attributes are not visibly listed in requirement documentation. They are hidden between the lines and difficult to decipher. Often time stakeholders have little idea about how a QA would affect the software unless an Architect helps them to see connection between requirement and QA. Architect has to bring QA forward and list them out. This helps an architect to focus on items which are keys to developing successful software architecture under given constraints.

## **A**rchitecturally **S**ignificant **R**equirements (ASR)

Refer [Requirement discovery and constraint Analysis under Business Technology Strategy](requirements_discovery_and_constraints_analysis.md){:target="_blank"} for how to do requirement discovery.

The first step in collecting ASR is to read the requirement documents carefully. Look for requirements that fall in one of the following categories:

1.  Allocation of responsibilities:
    1.  Find out how the responsibilities are allocated to various elements of software.
2.  Coordination Model
    1.  List out elements that must or must not coordinate
    2.  Determine properties of the coordination
    3.  Choose the communication method within or without the system.
3.  Data Model
    1.  How the data of the system should be created, stored, accessed, changed, destroyed etc.?
4.  Management of Resources
    1.  Decisions which affect resource management
5.  Mapping among architectural elements
    1.  Locate any identified mapping structure defined. For e.g. mapping of modules to runtime elements, runtime elements to processors etc
6.  Choice of Technology
    1.  Are there any technologies identified to be used? Is there a particular environment the system has to run?
7.  Binding Time decisions
    1.  This covers every other category listed above. In each case there is a binding time decision involved.
    2.  For e.g. in resource management, the system should be able to accept a new device that is plugged in at runtime.

## Quality Attribute Workshop (QAW)

The next step is to interview stakeholders. If the number of stakeholders is large one has to choose whom to talk to. This could be dependent on the size of the effect on the design of the system by stakeholders.

QAW is a method for talking to stakeholders in a pre-defined setting. The steps involved in QAW are as follows:

Step 1: QAW Presentation and Introduction.

This is done by QAW facilitator. QAW facilitator is mostly the software architect.

Step 2: Business Presentation

This is done by Management Representative. Aim is to explain the system's business context.

Step 3: Architectural Plan Presentation

This is done by architect. Architect provides a rough system architectural plan as it stands at that time

Step 4: Identification of Architectural Drivers.

Selection of drivers based on conversation in step 2 and 3 above. Ask the participants to clarify, add, and delete the drivers.

Step 5: Scenario Brainstorming

Architect should ensure that there is at least one Scenario for each driver in step 4.

Step 6: Scenario Consolidation

Stakeholders push backs are normal on non-functional requirements. An architect has to demonstrate how a QA is related to the requirement to avoid such push backs.  The stakeholders are not interested in spending on requirements that are not listed by them.

It is necessary to identify an ASR and the related QA to answer queries on non-functional requirements.  Cost-benefit of a QA and its role in architecture should be described in a layman's words to get stakeholders buy-in.

Stakeholders involve architect at an early stage to get the architecture correct from the current and future requirements perspective.

Stakeholders should understand that same requirement can have very different implementation from different people. Success depends on how well the ASR is identified and mapped to one or more QA. Since stakeholders are involved in for a long haul, they want continuity with the software in future. For the sake of using software for a long time it is necessary to involve an Architect early on because architecture cannot be changed at a later date and rewrite is very costly.

## Quality Attribute Scenario:

As seen above the writing of an appropriate QA Scenario is very important to get the ASR right. Quality attribute scenario has the following important parts:

1.  Who is Stimulating?
    1.  It could be a human, a computer, fault in the system etc
2.  What it does to the system?
    1.  It could be an event that occurs, an attack in progress etc
    2.  It could be a user clicking on the menu, typing in the text box etc
3.  What response to give to the stimulus received?
4.  How to measure the response?
    1.  Is it satisfactory to prevent the attack? Or, additionally, inform the people watching the system and log the information too?
    2.  In case of performance, is it sufficient to measure the latency? Or, need to look into the processing time too.
5.  What environment this stimulus occurs in?
    1.  Do we have control over the environment? Can we change it for the better?
    2.  If not, do we have to prepare our system to handle such issues better next time?
6.  Artifacts
    1.  Is it a specific component of the system that is affected or a sub-system?

Two characteristic comes if QA is written this way. One, since specific measurement of the response has to be documented, the scenario becomes testable. Second, since we know clearly the stimulus, response, environment it occurs in and the artifacts it affects, it is unambiguous.

## Quality Attribute Testing

The testing of QA differs from one attribute to another.  Some of them can be tested using Analytical model others need a checklist. In some cases one need to create model (prototype) to test. We will cover some of the QA here.

## Performance

Assume the software has used Model View Controller (MVC) design. We need to know the following information

-   Arrival rate of events
-   Selected Queue discipline
-   Selected scheduling algorithm
-   Service time for events
-   Network topology
-   What time it takes to process the message in view/model/controller
-   Bandwidth of the network connect to view/model/controller

With these details one can calculate the latency of the system.

## Security

In case of security mostly it is a checklist. The checklist is sourced from many sources. For e.g. for payment receiving websites it has to follow the checklist of Payment Card Industry (PCI) as part of their security checklist.

The checklist can also be sourced from internal to the company. For e.g. if company do not serve a particular country it may not permit log-in from that country. The security testing checklist should include a test around who can or cannot log-in including successful and failure tests. This is the access rights testing.

## Balancing and optimizing quality attributes

Refer [Balancing and Optimizing Quality attributes under Quality Attribute Pillar](boqa.md){:target="_blank"}

## Architecture Evaluation

The most common evaluation method is Architecture Trade-off Analysis Method(ATAM).

It has 4 phases as follows:

-   Partnership and preparation. Here the evaluation team leadership meet to list out the details for ATAM exercise. Information gathering for the exercise is done here.
-   (evaluation phase 1) This is a continuation of the phase one with more analysis.
    -   Details on business drivers
    -   During QAW the architecture was not detailed enough. By now the architect will be able to cover all necessary parts in enough details for the participants to evaluate the system.
    -   List out architectural approaches.
    -   Generate Quality Attribute Utility tree.
    -   Analyze approaches taken
-   Some more evaluation (evaluation phase 2)
    -   There is a gap between the first evaluation and this one.
    -   A summary of the first evaluation is created.
    -   More scenarios are analyzed if required.
    -   Brainstorming on scenarios takes place. Scenarios are prioritized.
    -   Architectural approaches are analyzed.
    -   Present the result of the evaluation to the stakeholders
-   Follow-up. Prepare final report and submit.

## Economic analysis of Quality Attributes

Also refer [Business Valuation under Business Technology Strategy](business_valuation.md){:target="_blank"}

When listing out various design strategies for a Quality Attribute the architect should be able to weigh the financial cost of the strategy too.

This starts with the QA Scenarios collected and refined in QAW and similar efforts. Then effort was put in to map architectural strategies to responses in scenarios.  There could be some side-effects on other QAs. The side-effects could be negative.  This leads to capture the utility of alternative responses in a scenario in a utility-response curve. With this curve it becomes easy to calculate the total benefit for a strategy. Estimate the cost of implementing the strategy. The ratio of total benefit and cost of implementing will give the Value of cost.  Use the ratio value to select the strategy to be implemented.

The process explained above is called Cost Benefit Analysis Method (CBAM).

# Sub-Capabilities

## Quality Attribute Discovery

Refer individual Quality Attributes under [Quality Attribute Pillar](qap.md){:target="_blank"}

| **Iasa Certification Level** | **Learning Objective** |
| **CITA - Foundation** | - Learner will be able to define Quality Attribute
| | - Learner will be able to define various Quality Attribute e.g. Security, Performance, Manageability, Usability etc.
| | - Learner will be able to compare and contrast Quality Attribute and requirements
| | - Learner will be able to reason why Discovery of Quality Attribute is important
| **CITA - Associate** | - Learner will be able to define ASR
| | - Learner will be able to list common methods of identifying ASR
| | - Learner will be able to define **P**edigreed **A**ttribute e**L**icitation **M**ethod (PALM)
| | - Learner will be able to list out benefits of PALM
| **CITA - Specialist** | - Learner will be able to list out major design decision categories to group requirement under to be specified as ASRs
| | - Learner will be able to list out steps involved in carrying out QAW
| | - Learner will be able to reason why business goals are important for Quality Attribute Discovery
| | - Learner will be able to list out important business goal categories
| **CITA - Professional** | - Learner will be able to identify challenges in identifying 'important' stakeholders?
| | - Learner will be able to provide information on why Architectural Plan presentation is important in a QAW
| | - Learner will be able to identify when to use which method - PALM , QAW

## Quality attribute scenarios

| **Iasa Certification Level** | **Learning Objective** |
| **CITA - Foundation** | - Learner will be able to define functions and quality of a system
| | - Learner will be able to contrast function and quality of a system
| | - Learner will be able to identify functionality scenarios and Quality Attribute scenarios?
| | - Learner will be able to list out why Quality Attribute Scenarios are required
| **CITA - Associate** | - Learner will be able to list out Quality Attribute scenarios main parts
| | - Learner will be able to list out basic requirements of a QA scenario
| | - Learner will be able to define architectural tactics
| | - Learner will be able to list out importance of architectural tactics in QA scenarios
| **CITA - Specialist** | - Learner will be able to reason why response measure be specified separately from response
| | - Learner will be able to identify performance QA in availability scenario
| **CITA - Professional** | - Learner will be able to  find dependency among QA while developing a particular QA scenario
| | - Learner will be able to list out how usability scenario would affect flexibility/security QA

## Quality Attribute Design Strategy

| **Iasa Certification Level** | **Learning Objective** |
| **CITA - Foundation** | - Learner will be able to list out characteristics of Attribute-driven design (ADD)
| | - Learner will be able to list out other design methods
| | - Learner will be able to list design checklist for Quality Attribute
| **CITA - Associate** | - Learner will be able to list required inputs for ADD
| | - Learner will be able to list outputs from ADD
| | - Learner will be able to enumerate steps in ADD
| | - Learner will be able to explain refinement strategies in ADD
| **CITA - Specialist** | - Learner will be able to map Architecturally Significant requirement(ASR) to design approaches
| | - Learner will be able to verify that all ASRs are accounted in ADD
| | - Learner will be able to create design decisions checklist for a QA. For e.g. Security
| **CITA - Professional** | - Learner will be able to develop design approaches for ASR |

## Software Architecture evaluation

| **Iasa Certification Level** | **Learning Objective** |
| **CITA - Foundation** | - Learner will be able to list out evaluation factors
| | - Learner will be able to reason how QA scenario would be useful for software evaluation
| **CITA - Associate** | - Learner will be able to list out methods used for software evaluation
| | - Learner will be able to list out steps involved in ATAM
| | - Learner will be able to identify stakeholders for ATAM
| **CITA - Specialist** | - Learner will be able to list important architectural views to be presented during ATAM
| | - Learner will be able to list out characteristic of Attribute-based architectural styles (ABAS)
| | - Learner will be able to draw utility tree for the project
| **CITA - Professional** | - Learner will be able to provide architectural decisions for a QA. For e.g. performance
| | - Learner will be able to provide weightage for each refinement of a QA in utility tree
| | - Learner will be able to present ABAS
| | - Learner will be able to brainstorm QA and help prioritize

## Quality Attribute Testing

| **Iasa Certification Level** | **Learning Objective** |
| **CITA - Foundation** | - Learner will be able to list out source of ideas for a QA testing
| | - Learner should know the reason for QA testing
| **CITA - Associate** | - Learner will be able to identify and list out QA testing separate from functional testing |
| **CITA - Specialist** | - Learner wil be able to identify required information for a particular QA testing
| | - Learner should be able to identify methods required to test a QA
| **CITA - Professional** | - Learner will be able to list out testing requirements for a particular QA testing |

# Related Capabilities

-   Business Technology Strategy Pillar
    -   Business Valuation
    -   Requirement Discovery and constraint analysis
-   Design
    -   Requirement Modeling
-   IT Environment
    -   Testing methods, tools, and techniques
-   Quality Attribute Pillar
    -   Balancing and Optimizing Quality Attributes
    -   Performance, Reliability, Availability, Scalability
    -   Security
    -   Usability et al

# Resources

**Articles:**

[SEI Quality Attribute Workshop - 3rd Edition](http://resources.sei.cmu.edu/library/asset-view.cfm?assetID=6687){:target="_blank"}

[Architecture Best Practices for Project and Technical Leaders](http://resources.sei.cmu.edu/asset_files/Presentation/2014_017_101_423682.pdf){:target="_blank"}

[Architecturally Significant Requirements - Paul Preiss](https://btabok.iasaglobal.org/architecturally-significant-requirements/){:target="_blank"}

[Classification of Software Prototyping](http://resources.sei.cmu.edu/asset_files/TechnicalReport/1992_005_001_16067.pdf){:target="_blank"}

**Blogs/Webcasts/News/Reference sources:**

[IASA Foundation BTABoK](https://btabok.iasaglobal.org){:target="_blank"}

[Software architecture in Practice-3rd Edition](http://resources.sei.cmu.edu/library/asset-view.cfm?assetid=30264){:target="_blank"}

[Microsoft Application Architecture Guide-2nd Edition-2009](https://msdn.microsoft.com/en-us/library/ee658094.aspx){:target="_blank"}

[Evaluating Software Architecture](http://resources.sei.cmu.edu/library/asset-view.cfm?assetid=30698){:target="_blank"}

# Author

**Sanjay Mishra**