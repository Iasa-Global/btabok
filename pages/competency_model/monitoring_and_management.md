---
title: "Monitoring and Management"
keywords: 
sidebar: mydoc_sidebar
toc: true
permalink: monitoring_and_management.html
folder: competency_model
summary: "An architect must design solutions with monitoring and management thought out from the beginning."
tags:
  - quality_attributes
---

# Description

Throughout the project lifecycle, the architect ultimately owns the delivery of quality attributes (a.k.a. non-functional attributes like security, availability, performance, scalability, etc.) to meet a solution's business requirements. Those requirements drive the need to discuss quality attribute tradeoffs. The architect must lead the discussion on quality attribute tradeoffs.

The decisions around quality attributes must be monitored and managed throughout the project lifecycle. As an architect manages how the quality attributes are being implemented, he must communicate at the enterprise executive level with artifacts from a business impact viewpoint.

Cloud Computing is a forcing function to better define the relationship between providers and consumers, providing more visibility into contract SLAs, scaling, monitoring instrumentation, and management interfaces.

# Overview

An architect must design solutions with monitoring and management thought out from the beginning. Solutions "designed for operations" can be deployed, monitored, operated, maintained, and scaled according to the organization requirements. Monitoring and management comprise quality management imperatives, techniques, and tools. This capability requires proficiency in problem analysis, capacity planning, instrumentation and monitoring, service level agreement (SLA) creation and management, and issue response techniques

The architect's ownership on quality attribute tradoffs translates to different tasks, depending on the architect's domain area:

-   Software or Infrastructure
    -   Leading a team in making quality attribute tradeoffs.
    -   Implementing a quality attribute tracking mechanism across projects and throughout the enterprise.
    -   Attaching system to quality attribute metric process and providing considerations on tools and process to manage updates for operating systems, hardware and applications
    -   Justifying financial value of quality attributes
    -   One of the strategies to manage both individual components and end-user service status is to design a health model representing all dependencies between components, from the physical layer up to the application layer. Management tooling must be able to provide real-time status of a service represented by the health model and alerts in case of a component failure, highlighting the impact to the service.
-   Business
    -   Continually monitoring quality attribute allocation for line of business or capability
    -   Ensuring stakeholder awareness of financial value of quality attribute goals
-   Information
    -   Ensuring quality attribute delivery for information usability across the enterprise
    -   Directing data and information quality attribute guidelines for access, retrieval, and storage

The architect should instrument the measurement of quality attributes. Quality assurance processes will then be able to compare delivered metrics to specified requirements. An SLA cannot be enforced without proper instrumentation. Adequate monitoring also allows early issue responses and avoids escalations that can potentially lead to low quality perception of a solution.

A new solution should be integrated to existing monitoring tools and processes, whenever possible. If the environment cannot provide appropriate monitoring tools or if the management processes in place cannot absorb the system, the architect must mitigate the gap. This can be achieved by deploying COTS monitoring and management packages and by training the operations team.

# Corporate Proven Practices

Governance allows project oversight for alignment to business needs and compliance to regulations. Architects must participate in the governance process and avoid disconnecting from the decision-making framework. Monitoring and management are quality attributes that provide verifiable parameters to the governance process.

# Sub-Capabilities 

## IT Service Management (ITSM)

ITSM refers to the implementation and management of quality information technology services. IT service providers perform ITSM through people processes, and information technology. ITSM is process-focused and tied to process improvement frameworks and methodologies like ITIL, TQM, Six Sigma, and CMMI.

| **Iasa Certification Level** | **Learning Objective** |
| :-: | :-: |
| **CITA- Foundation** | -   Learner will be able to define ITSM
| | -   Learner will be able to define availability
| **CITA -- Associate** | -   Learner will be able to describe two ITSM frameworks at a high-level
| | -   Learner will be able to discuss service level management
| | -   Learner will be able to discuss problem management
| | -   Learner will be able to discuss incident management
| | -   Learner will be able to give examples of availability measurements
| **CITA -- Specialist** | -   Learner will be able to demonstrate proficiency in ITIL or another recognized ITSM framework
| | -   Learner will be able to demonstrate practice in at least one ITSM tool
| | -   Learner will be able to assess measurements and metrics in place and evaluate if the level of service satisfies compliance and business objectives
| **CITA -- Professional** | -   Learner will be able to compare and evaluate different ITSM frameworks
| | -   Learner will be able to compare and evaluate different high-availability strategies

## Service Level Agreement (SLA)

Service level agreement (SLA) is a documented agreement between the service provider and the customer that identifies services and service targets -- ISO 20000-1 (2011).

| **Iasa Certification Level** | **Learning Objective** |
| :-: | :-: |
| **CITA- Foundation** | -   Learner will be able to define service level agreement (SLA)
| | -   Learner will be able to explain the difference between SLA and operational level agreement (OLA)
| **CITA -- Associate** | -   Learner will be able to identify elements in an SLA
| | -   Learner will be able to identify elements in an OLA
| | -   Learner will be able to discuss SLA management and QoS (quality of service) parameters
| | -   Learner will be able to describe multi-tiered solution support (levels 1, 2, 3)
| **CITA -- Specialist** | -   Learner will be able to defend an SLA to peers
| | -   Learner will be able to describe maintenance procedures for a solution
| | -   Learner will be able to differentiate between Master Service Agreement, Service Agreement, and SLA
| **CITA -- Professional** | -   Learner will be able to model an SLA
| | -   Learner will be able to demonstrate proficiency in SLA creation and management
| | -   Learner will be able to demonstrate proficiency in issue response techniques

## Monitoring

Monitoring is awareness of the state of a system.

| **Iasa Certification Level** | **Learning Objective** |
| :-: | :-: |
| **CITA- Foundation** | -   Learner will be able to define monitoring
| | -   Learner will be able to recognize the basic set of quality attributes
| **CITA -- Associate** | -   Learner will be able to explain how a quality attribute can be monitored
| | -   Learner will be able to recognize COTS monitoring tools
| **CITA -- Specialist** | -   Learner will be able to practice monitoring quality attributes
| | -   Learner will be able to select which quality attributes to monitor
| | -   Learner will be able to implement a quality attribute tracking mechanism for a solution
| | -   Learner will be able to demonstrate proficiency in a monitoring tool that is relevant to a domain area
| **CITA -- Professional** | -   Learner will be able to evaluate quality attribute trade-offs
| | -   Learner will be able to justify financial value of quality attributes

## Capacity Management

Capacity management is a process that ensures the IT capacity meets current and future business requirements in a cost-effective manner.

| **Iasa Certification Level** | **Learning Objective** |
| :-: | :-: |
| **CITA- Foundation** | -   Learner will be able to define capacity management
| | -   Learner will be able to describe high-level activities related to capacity management, according to the ITIL framework
| **CITA -- Associate** | -   Learner will be able to track direct business benefits arising from a technology solution
| | -   Learner will be able to classify benefits and value additions
| **CITA -- Specialist** | -   Learner will be able to discuss the impact of capacity management
| | -   Learner will be able to discuss how performance management and capacity management are related
| | -   Learner will be able to describe the relationship between capacity management and proper risk assessment for business continuity planning (BCP
| **CITA -- Professional** | -   Learner will be able to model a capacity planning strategy
| | -   Learner will be able to choose between capacity planning strategies
| | -   Learner will be able to justify the business value of a capacity planning strategy

# Resources

**Articles:**

IASA BTABOK -- [https://btabok.iasaglobal.org](https://btabok.iasaglobal.org){:target="_blank"}

ISO/IEC 20000-1:2011: Service management system requirements -- [http://www.iso.org/iso/catalogue_detail?csnumber=51986](http://www.iso.org/iso/catalogue_detail?csnumber=51986){:target="_blank"}

NIST: SP 800-146 -- Cloud Computing Synopsis and Recommendations -- [http://csrc.nist.gov/publications/nistpubs/800-146/sp800-146.pdf](http://csrc.nist.gov/publications/nistpubs/800-146/sp800-146.pdf){:target="_blank"}

NIST: Cloud Service Level Agreements -- Meeting Customer and Provider needs -- [https://www.nitrd.gov/nitrdgroups/images/3/34/SLA_Overview_FASTER_20140128.pdf](https://www.nitrd.gov/nitrdgroups/images/3/34/SLA_Overview_FASTER_20140128.pdf){:target="_blank"}

European Commission: Cloud Computing Service Level Agreements -- [http://ec.europa.eu/digital-agenda/en/news/cloud-computing-service-level-agreements-exploitation-research-results](http://ec.europa.eu/digital-agenda/en/news/cloud-computing-service-level-agreements-exploitation-research-results){:target="_blank"}

ITIL: Continual Service Improvement -- [https://www.ucisa.ac.uk/~/media/Files/members/activities/ITIL/continual_service_improv/ITIL_Introducing%20Continual%20Service%20Improv%20pdf.ashx](https://www.ucisa.ac.uk/~/media/Files/members/activities/ITIL/continual_service_improv/ITIL_Introducing%20Continual%20Service%20Improv%20pdf.ashx){:target="_blank"}

**Books:**

Hill, Joyce (2006) -- *Capacity Requirements Planning*

# Author

![Alberto Boczar](media/a_boczar.jpg)
**Alberto Boczar**
*Infrastructure Architect -- Microsoft*

Alberto Boczar is an Infrastructure Architect in Microsoft Services HQ in Redmond, WA. He is the Chief Architect in a team developing worldwide services offerings and solutions based on Microsoft products, technologies, and cloud services like Azure, so that consultants and architects can provide expertise to Microsoft customers and partners, for maximum return on their investment in Microsoft products and technologies.

Before moving to Redmond, Alberto worked as a consultant for Microsoft Brazil. Prior to joining Microsoft in 2005, Alberto worked as a consultant for a Microsoft partner in Brazil, designing, deploying and supporting infrastructure, identity, and messaging solutions. He also worked for Unisys Brazil as a support engineer.

Alberto has 28 years of experience in the IT industry. He holds a bachelor's degree in Electrical Engineering, and certifications from Microsoft and IASA.

