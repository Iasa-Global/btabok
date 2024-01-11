---
title: "Security"
keywords: 
sidebar: mydoc_sidebar
toc: true
permalink: security.html
folder: competency_model
summary: "Security is a universal quality attribute to manage risk to the confidentiality, integrity, or availability of information or systems."
tags:
  - quality_attributes
---

# Description

Security is a complex quality attribute which has developed into a capability with specialized architects.  Security as a quality attribute represents the mitigation of threats and vulnerabilities to confidentiality, integrity, or availability of the data in a system or the systems themselves.  In order to enhance delivery against this quality attribute, the architect will need to understand potential risks, the technology, process, and people capabilities needed to mitigate those risks, and be able to identify appropriate tradeoffs with cost and system functionality.

In recent years, managing the Security of a system will require architects to have closely related design and understanding of options for system performance, availability, meeting compliance criteria, and the advent of Privacy as a quality attribute.

# Overview

## Why does an architect need this skill? 

Security is a "universal" quality property. That is, it is present in all systems, even small, simple ones.  The architect should be aware of that, and needs to have the "security awareness", a state that will detect security requirements in regular, common scenarios, even when no security seems to be needed. That is because security relates not only to authentication, but also on quality of delivery, availability and several other "illities"

## Common tasks involved in this skill?

All architects need a basic understanding of strategies for availability for a system, and to understand a basic requirements gathering process for potential vulnerabilities, high likelihood threats, and compliance requirements for the protection of a system and its data.  Security awareness should be included in architecture and design approaches from stage 0 (stating the business context). The architect must understand business needs and identify the security requirements aligned with the business strategy. The architect needs to comply with regulations, establish security models and frameworks, review correct design and coding practices, and assure security is present during operation and sunset of systems.

## What is their ownership in this skill?

The architect is the closest link to the system implementation in a  security chain that starts with the business goals and strategy, the stakeholder and security officers if they exist at the organization.

Name an example of how an architect would use this in daily activities?

An online sales company wants to expand its operations and become international. Apart from ensuring the use of the best security practices to provide confidentiality, integrity and availability, the architect must also understand the requirements in this strategy, take into account regulations on the target countries regarding information use and distribution, the regulations and compliance to industrial payment standards, the effect on availability of the increased number of clients, etc.

# Best Practices

## Describe why an architect should be involved in this skill at a corporate level

Security is not a technology only issue, it relates to the obligations of the business and the composite people, processes AND technologies that realize the business intent. The impact of a security breach affects business in several ways, from an impact to the company image and trust, to the loss of money due to non-operation periods. Still, security is mainly realized using technology means and the operation and monitoring of system information.  To mitigate risk in realizing the business targeted results, an architect will need either deep skill in designing for these needs or to partner with specialists inside or outside the organization to ensure th requirements for the system's security are gathered, prioritized, and capabilities included to meet these needs.

## Primary push back and/or challenges for architects

Security is usually thought as an identification/authorization problem. It is also taken as a afterthought, something to be added later. To create a robust architecture, the architect needs to understand and make understandable to stakeholder, the complexity of security, risk and planning.  This complexity, too, can be a difficulty as people with the neccessary skills, and increases in cost to meet security needs can be challenging to the organization.

## How would a stakeholder engage an architect for assistance utilizing this skill?

As mentioned, security is almost a universal topic, present in all systems. It should be part of every requirement/scenario/use case review. Sadly, more than often the topic is mentioned after a problem or attack has been detected.  Organizations should include security and privacy obligations as part of the design cycle, identify the magnitude and type of risks which are not tolerable to the intended outcomes of the system, and identify capabilities that mitigate, avoid, or transfer intolerable risk.

# Sub-Components Skills

## Secure Component Skills:

This includes but is not restricted to: common and/or standardized security models and methodologies, authorization models, knows security related frameworks, hacking methodologies, the C.I.A. acronym (Confidentiality, Integrity and Availability), risk evaluation concepts.

| **Iasa Certification Level** | **Learning Objective** |
| :-: | :-: |
| **CITA- Foundation** | -   Learner will be able to explain what the C.I.A. acronym stands for.
| | -   Learner will be able to explain what is risk management and why is it important
| | -   Learner will be able to name some of the most known security standards
| | -   Learner will be able to name common security methodologies.
| | -   Learner will be able to name the security models or patterns most relevant to the type of architecture they are engaged in, like walled garden, zero trust architecture, etc.
| **CITA -- Associate** | -   Learner will be able to explain the design flow from conceptual to implementation description of architecture artifacts.
| | -   Learner will be able to explain how to transform collected architectural information and intents into viable models.
| | -   Learner will be able to depict functional requirements of the architecture.
| | -   Learner will be able to explain the key patterns used to mitigate risk in the architectural description.
| **CITA -- Professional** | -   Learner will be able to conduct a threat modeling process
| | -   Learner will be able to apply some security threat modeling approaches, like OCTAVE, STRIDE, DREAD, and apply industry published bodies of work that organize attack patterns like ATT&CK and ATLAS.
| | -   Learner will be able to identify likely regulatory and compliance obligations that would affect a system in the context of that system's implementer, geography, and industry.
| | -   Learner will be able to create architectures that are compliant to different standards from NIST, ISO, regulators for an industry or country etc.
| | -   Learner will be able to implement a suitable security model.
| | -   Learner will be able to synthesize security adoption approaches to enhance the likelihood of successful risk mitigation in the implemented system..
| **CITA -- Distinguished** | -   Learner will be able to define and implement risk management in the enterprise and guide other architects in established processes, approaches, and patterns to mitigate similar risks
| | -   Learner will be able to implement and comply with security best practices indicated in known frameworks, like COBIT
| | -   Learner will be able to identify the impact of the use of different security models for systems enterprise wide.

## Security in Requirements

Methods and techniques to elicit security requirements evaluate them and prioritize them along the business strategy. Includes generation of negative requirements, abuse cases, risk management and threat modeling.

| **Iasa Certification Level** | **Learning Objective** |
| :-: | :-: |
| **CITA- Foundation** | -   Learner will be able to explain what an abuse case is.
| | -   Learner will be able to explain what sources of security requirements are.
| | -   Learner will be able to explain what a subject-object matrix is
| | -   Learner will be able to explain what "protection need elicitation" means
| **CITA -- Associate** | -   Learner will be able to extract security requirements from positive requirements
| | -   Learner will be able to explain different authorization requirements types (DAC, NDAC, MAC, RBAC, etc).
| | -   Learner will be able to identify different types of requirements (integrity, auditing, session management, archiving, antipiracy, etc).
| **CITA -- Professional** | -   Learner will be able to conduct Protection Needs Elicitation procedures, like policy decomposition, data classification, misuse and abuse case modeling S-OM.
| | -   Learner will be able to identify the access control method to use in different cases
| **CITA -- Distinguished** | -   Learner will be able to identify, capture, manage, security requirements enterprise wide
| | -   Learner will be able to prioritize and perform a trade-of process to select security requirements to implement based on the business strategy and resources.

## Security in Architecture and Design

Security analysis at architectural level, description of solution using improved architectural views, the security perspective (Woods/Rozanski), security in architectural styles. Also security design principles.

| **Iasa Certification Level** | **Learning Objective** |
| :-: | :-: |
| **CITA- Foundation** | -   Learner will be able to explain the Security Perspective (Woods/Rozanski).
| | -   Learner will be able to explain the different security implications in known architecture styles (SOA, REST among them)
| | -   Learner will be able to name some of the most known security design principles.
| **CITA -- Associate** | -   Learner will be able to balance the different design principles.
| | -   Learner will be able to explain the design considerations related to security, including confidentiality, integrity, availability, authentication, authorization, auditing.
| | -   Learner will be able to explain the issues and solutions of Identity architecture.
| | -   Learner will be able to the implication of security in database design
| **CITA -- Professional** | -   Learner will be able to implement technologies like identify management, certificate management, IDS, IPS, Virtualization, DRM
| | -   Learner will be able to identify issues and implement security adjustments for different types of architectures, like web applications, SaaS, RIA, pervasive computing, etc.
| | -   Learner will be able to perform an attack surface evaluation.
| **CITA -- Distinguished** | -   Learner will be able to evaluate the impact on business of each design decision and balance the cost benefit.

## Security in Implementation

Knowledge of security issues in different languages, workarounds, common software vulnerabilities, defensive programming, security code smells, security in the software process.

| **Iasa Certification Level** | **Learning Objective** |
| :-: | :-: |
| **CITA- Foundation** | -   Learner will be able to name the most common software vulnerabilities.
| | -   Learner will be able to name the different development methodologies and explain how security should be incorporated in each of them.
| | -   Learner will be able to name the different defensive coding practices
| | -   Learner will be able to explain the importance of exception handling
| | -   Learner will be able to name security issues related to different coding languages.
| **CITA -- Associate** | -   Learner will be able to explain how the common vulnerabilities can be exploited and name the most common solutions to avoid or minimize the issue.
| | -   Learner will be able to explain the importance of security in the regular development processes like code analysis, peer reviews and configuration management.
| **CITA -- Professional** | -   Learner will be able to indicate the best development practices to be used during development.
| | -   Learner will be able to incorporate security during the corresponding development methodology
| **CITA -- Distinguished** | -   Learner will be able to evaluate the impact of vulnerabilities and solutions to strategy, and explain the long term impact to stakeholders.

## Security in Acceptance

Evaluation of required acceptance level for security, acceptance testing, certification and accreditation.

| **Iasa Certification Level** | **Learning Objective** |
| :-: | :-: |
| **CITA- Foundation** | -   Learner will be able to distinguish between certification and accreditation concepts.
| | -   Learner will be familiar with the build configurations to be validated for deployment or release
| | -   Learner will be able to list the procurement considerations for deployment or release acceptance
| | -   Learner will be able to explain why assurance in acquisitions and legal protection mechanism are needed for software procurement.
| **CITA -- Associate** | -   Learner will be able to define the acceptance criteria for pre and post deployment/release
| | -   Learner will be able to understand how Validation and Verification can be used for Certification and Accreditation
| **CITA -- Professional** | -   Learner will be able to explain the relation between software assurance an the acceptance criteria for pre and post deployment/release.
| | -   Learner will be able to understand what a software escrow is and why is needed.
| **CITA -- Distinguished** | -   Learner will be able to verify that the measures of the impact of the software to be deployed to the exiting computing ecosystems is being taken and analyzed.
| | -   Learner will be able to understand when a software escrow strategy is needed and implement it. 

## Security in Deployment, Operations, and Disposal

Environment hardening, penetration testing, problem and incident management, problem detection, monitoring, information protection and destruction.

| **Iasa Certification Level** | **Learning Objective** |
| :-: | :-: |
| **CITA- Foundation** | -   Learner will be able to understand the concepts of hardening, bootstrapping and secure startup.
| | -   Learner will be able to explain what continuous monitoring is.
| | -   Learner will be able to understand what a security incident is.
| | -   Learner will be able to understand the importance of good disposal planning in terms of security
| **CITA -- Associate** | -   Learner will be able to understand the configuration management concepts and they relation with security
| | -   Learner will be able to explain what incident management is
| | -   Learner will be able to explain what a patching strategy is
| | -   Learner will be able to explain what a root cause analysis is
| **CITA -- Professional** | -   Learner will be able to define the requirements for the implementation of the incident management, patching and problem detection strategies.
| | -   Learner will be able to ensure the compliance with end-of-life (EOL) policies for software systems.
| | -   Learner will be able to ensure the hardening of software and hardware is in place and working as expected.
| **CITA -- Distinguished** | -   Learner will be able to explain why strategies for continuous monitoring, problem detection and incident management should be aligned to the business strategy and goal.
| | -   Learner will be able to align EOL policies to external regulations

## Business continuity and disaster recovery planning

As part of the Availability concern (from the C.I.A. acronym), the architect needs to know about critical business process protection, business continuity planning and execution, disaster detection, containment and recovery. These topics are covered in other capabilities, like the Availability Quality Attribute in 'Performance, Reliability, Availability, Scalability' and Disaster Recovery in Disaster Recovery and Backup.

## Security Regulations and Compliance

Industrial, geographical and political regulations are to be known and understood.

| **Iasa Certification Level** | **Learning Objective** |
| :-: | :-: |
| **CITA- Foundation** | -   Learner will be able to explain why there should be regulatory, privacy and compliance requirements.
| | -   Learner will be able to list the different security standards (NIST, ISO, etc) and types (Industry, Government, International and National)
| | -   Learner will be able to describe the benefits of following the different security standards
| **CITA -- Associate** | -   Learner will be able to list the significant regulations and acts, namely SOX, BASEl II, GLBA, HIPAA, Data protection Act, Computer miuse Act, etc.
| | -   Learner will be able to explain what a Acceptably Use Policy (AUP) is and why is it important for privacy and software development
| **CITA -- Professional** | -   Learner will be able to understand and apply the different regulations and acts in software architecture definition
| | -   Learner will be able to define an architecture the complies with AUP
| **CITA -- Distinguished** | -   Learner will be able to explain how regulations impact the business strategy and plan for a remedial solution
| | -   Learner will be able to measure the impact of regulations for globally used/distributed systems.

# Capabilities Resources

**Articles**

**Blogs/Webcasts/News Sources**

**Training**

-   CISM Review Courses [http://www.isaca.org/Certification/CISM-Certified-Information-Security-Manager/Prepare-for-the-Exam/Review-Courses/Pages/default.aspx](http://www.isaca.org/Certification/CISM-Certified-Information-Security-Manager/Prepare-for-the-Exam/Review-Courses/Pages/default.aspx){:target="_blank"}
-   ISC2 courses [https://isc2.org/elearning/default.aspx](https://isc2.org/elearning/default.aspx){:target="_blank"}

**Certifications**

-   (ISC)2 CISSP
-   (ISC)2 CSSLP
-   IASACA CISM

**Books**

-   Paul Mano, Official ISC2 Guide to the CSSLP
-   Adam Gordon, Official ISC2 Guide to the CISSP CBK
-   Gary McGraw, Software Security: Building Security In
-   Ron McFarland, INFORMATION SECURITY BASICS: FUNDAMENTAL READING FOR INFOSEC INCLUDING THE CISSP, CISM, CCNA-SECURITY CERTIFICATION EXAMS

# Author

**William Martinez**
*R&D Manager -- Avanta Technologies*

