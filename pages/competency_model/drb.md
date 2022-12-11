---
title: "Disaster Recovery and Backup"
keywords: 
sidebar: mydoc_sidebar
toc: true
permalink: drb.html
folder: competency_model
summary: "IT is often tasked with creating disaster recovery plans and also assists with business continuity planning (BCP)"
tags:
  - infrastructure_architecture
---

# Description

Disaster recovery (DR) is part of Business continuity management framework that deals with protecting an organization from the effects of significant negative events, both internal and external in nature. Such as equipment failures, fire, cyber-attack, and hurricanes. Any event that could significantly impact business operation should be included in a disaster recovery planning. Although DR traditionally overlooked, however given the high number of natural and man-made disasters in the past decade many organizations are adopting the approach that disaster recovery is a must have rather than a nice to have.

Backup is the process of backing up corporate data either locally in the same data center (some time termed near disk backup) or remotely such as the case of replicating the data to tape and storing them offsite. Data backups are simply taking periodic snapshot of your data for restoration purpose in case of an accidental deletion or data corruption. It is critical to understand that data backup does not constitute disaster recovery planning, but could be one of the pillars of such a plan.

It is worth noting that "Business Continuity Planning (BCP) and Disaster Recovery (DR) are used interchangeably, however there is a difference between the two. BCP refers to plans about how the business resume operations in case of a disaster this includes both IT operations and business processes associated with providing a service. DR refers to how IT (information technology) should recover in case of a disaster. In summery BCP is more holistic and DR is usually a subset of BCP.

# Overview

## Why Does an Architect need this Skill?

Webopieda defines an IT architect as follows:

"An Information Technology Architect is the individual responsible for linking computer technology decision making and investments with an organization's tech business strategy.  The individual is responsible for organizing a consensus of decisions on policies, principles, services, standards, guidelines, and common solutions for the betterment of the company or organization. IT Architects are responsible for guiding the process of planning acquiring, building, modifying, and deploying IT resources throughout a given department."

IT is often tasked with creating disaster recovery plans and also assists with business continuity planning (BCP) for an existing process or a line of business. As defined above, IT architects being the focal point of IT delivery frame work, as such it is imperative they have a broad spectrum of IT skill sets including understanding and the ability to drive backup strategy, DR and BCP planning.

Disaster recovery and business continuity planning are a critical part of every organizations survival, as an architect it imperative that he/she evangelize the importance of these initiative both on a strategic level from a roadmap prospective and a tactical level on specific initiatives or projects. Having the proper knowledge and understanding of the different aspects of DR will allow the architect to articulate the importance and the need for such a risk mitigation strategy.

## Common tasks involved in this Skill.

The architect will be involved in multiple phases of disaster recovery, backup and business continuity planning

-   Assist in assembling disaster recovery team the team should consist of various technical and business stockholders and lines of business in the scope of the DR. The architect should obtain a high level business sponsor to endorse the plan upon completion.
-   The architect will assist in defining risk profile for the enterprise and prioritizing risk based on probability and impact. Risks with highest impact and highest probability should be mitigate first.
-   Assist in preforming BIA (business impact analysis) to identify what needs to be protected by a disaster recovery plan. BIA should be performed on line of business or functional area (finance, customer service, etc.) That needs to be protected.
-   Translate business requirement into an RPO (return point objective) and RTO (return time objective).
-   Architect a solution that meets RPO and RTO requirements defined above. Involve engineering and operations team in the architectural design to ensure effective and agreed on solution across the design, build and run technology stack.
-   Build Disaster recovery plan based on the list of assets and/or services to be protected and the BIA assessment preformed.
-   Create recovery procedure that includes step-by-step plan that goes through both the failover and failback procedure. The plan should clearly define roles and responsibilities.
-   Assist in planning a DR test, during this step the engineering team will perform a DR test, the architect should monitor and evaluate the procedure and steps to ensure that it meets defined requirements and modify procedure or architecture if deemed necessary.
-   DR plan is a continuously evolving document and should be reviewed at set intervals to ensure validity of assumption and requirements. The architect should review the document at set interval and suggest changes as they see fit.

## What is their Ownership in this skill?

The architect(s) will lead the architectural aspect of the recovery solution, as well as guiding the organization in driving the recovery parameters. In larger organizations there might be multiple architects with different areas of expertise involved in the recovery exercise, you might have a capacity architect addressing resource requirements, infrastructure architecture addressing the core infrastructure solution and a solution or enterprise architect addressing the overall solution. In smaller or even medium organizations the architect assigned to the project will perform all the aforementioned tasks

## How is this skill used by the architect in daily activities?

The Architect would be expected to be able to:

-   Understand the requirements to build a viable disaster recovery plan.
-   Understand the organizational requirements as well as any governance and/or legal requirements.
-   Understand which business function plays a pivotal role and as such DR/BCP plan may have more of a focus on system recovery related to these areas.
-   Understand both physical and logical requirement to achieve required RTO and RPO.
-   Communicating the DR plan to the stockholders.
-   Understand different technology offerings in the market place, understanding DR technology landscape will allow the architect ability to design and/or recommend appropriate solution(s).
-   Ability to translate business requirement to technical design.

# Proven Practices

**Describe why an architect should be involved in this skill at a corporate level?**

As defined above the architect is responsible for linking technology decisions with business strategy. It is increasingly evident that technology and the business cannot operate independently and there is a paradigm shift from perceiving IT as a cost center to IT as a business enabler. Solution or enterprise architect is uniquely positions to bridge the gap between business requirements and technical reality.

# Sub-Capabilities

## Business IMPACT ANALysis 

Initial step in DR/BCP planning process and should include the: Assessment and prioritization of all business functions and processes, including their interdependencies.

| **Iasa Certification Level** | **Learning Objective** |
| :-: | :-: |
| **CITA- Foundation** | -   The Learner should be able to identify the key requirements for DR and BCP planning.
| **CITA -- Associate** | -   The Learner is able to articulate the key considerations in the DR/BCP planning including RTO and RPO definition.
| | -   The Learner is able to speak to the different processes and interdependencies between these processes.
| **CITA -- Specialist** | -   The Learner will be able to demonstrate working knowledge of different business impact analysis processes.
| | -   The Learner is able to discuss the architectural implications of DR/BCP plans, including capacity planning, data and networking implication
| | -   The leaner is able to articulate the finding of the business impact analysis to various stockholders.
| | -   The leaner is able to articulate cost implication of the defined RPO/RTO analysis. Also the ability to articulate cost/benefit analysis based on various RPO/RTO parameters.
| **CITA -- Professional** | -   The Learner will have experience with delivering architectural programs leveraging complex environments and can discuss working with engineering and operational teams
| | -   The Learner has experience developing and building DR/BCP plan based on the business impact analysis
| | -   The Learner has an ability to change their DR/BCP plans based on findings from business impact analysis and cost analysis.

# Resources

[https://en.wikipedia.org/wiki/Disaster_recovery](https://en.wikipedia.org/wiki/Disaster_recovery){:target="_blank"}

[Home](https://www.disasterrecovery.org/){:target="_blank"}

[http://www.ready.gov/business/implementation/IT](http://www.ready.gov/business/implementation/IT){:target="_blank"}

# Author

![Nabeel Yousif](media/n_yousif.jpg)
**Nabeel Yousif**
*Chief Architect, IT at Brinks Inc*

Nabeel Yousif is the Chief Architect, IT for Brinks Inc, in his role Nabeel is responsible for defining Global infrastructure strategic roadmaps such as cloud initiatives, DRaaS and virtualization. Prior to assuming this role Nabeel was responsible for the global system engineering group within Brinks and the Canadian infrastructure team.

Nabeel has 20 years of experience in the IT industry and holds a Bachelor's of Science degree in Physic and Computer Science from the University of Toronto. Nabeel also hold multiple industry certifications including CISSP and PMP.