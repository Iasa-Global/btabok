---
title: "Security"
keywords: 
sidebar: mydoc_sidebar
toc: true
permalink: security.html
folder: competency_model
summary: "Security is one universal quality property."
tags:
  - quality_attributes
---

# Description

Demonstrated understanding of security concepts and the application of best security practices during the whole system life cycle. Demonstrated understanding of regulations and compliance, security administration and business continuity assurance. Demonstrated competence in basic implementation techniques.

# Overview

## Why does an architect need this skill? 

Security is one "universal" quality property. That is, it is present in all systems, even small, simple ones.  The architect should be aware of that, and needs to have the "security awareness", a state that will detect security requirements in regular, common scenarios, even when no security seems to be needed. That is because security relates not only to authentication, but also on quality of delivery, availability and several other "illities"

## Common tasks involved in this skill?

The architect should understand what security is about, and include security awareness from stage 0 (stating the business context). The architect must understand business needs and identify the security requirements aligned with the business strategy. The architect needs to comply with regulations, establish security models and frameworks, review correct design and coding practices, and assure security is present during operation and sunset of systems.

## What is their ownership in this skill?

The architect is the closest link to the system implementation in a special security chain that starts with the business goals and strategy, the stakeholder and the security officers.

Name an example of how an architect would use this in daily activities?

For instance, an online sales company wants to expand its operations and become international. Apart from ensuring the use of the best security practices to provide confidentiality, integrity and availability, the architect must also understand the requirements in this strategy, take into account regulations on the target countries regarding information use and distribution, the regulations and compliance to industrial payment standards, the effect on availability of the increased number of clients, etc.

# Best Practices

## Describe why an architect should be involved in this skill at a corporate level

Security is not a technology only issue, it relates primarily to business. The impact of a security breach affects business in several ways, from an impact to the company image and trust, to the loss of money due to non-operation periods. Still, security is mainly enforces using technology, and security in technology is a very complex area. This is why architects should need this skill in a corporate facing analysis of security needs.

## Primary push back and/or challenges for architects

Security is usually thought as an identification/authorization problem. It is also taken as a afterthought, something to be added later. To create a robust architecture, the architect needs to understand and make understandable to stakeholder, the complexity of security, risk and planning.

## How would a stakeholder engage an architect for assistance utilizing this skill?

As mentioned, security is almost a universal topic, present in all systems. It should be part of every requirement/scenario/use case review. Sadly, more than often the topic is mentioned after a problem or attack has been detected.

# Sub-Components Skills

## Secure Component Skills:

This includes but is not restricted to: most know security models and methodologies, authorization models, knows security related frameworks, hacking methodologies, the C.I.A. acronym (Confidentiality, Integrity and Availability), risk evaluation concepts.

| **Iasa Certification Level** | **Learning Objective** |
| :-: | :-: |
| **CITA- Foundation** | -   Learner will be able to explain what the C.I.A. acronym stands for.
| | -   Learner will be able to explain what is risk management and why is it important
| | -   Learner will be able to name some of the most known security standards
| | -   Learner will be able to name common security methodologies.
| | -   Learner will be able to explain what Trust Computing means
| | -   Learner will be able to name the different security models, like BLP, Biba, Chinese Wall, etc.
| **CITA -- Associate** | -   Learner will be able to explain the design flow from conceptual to implementation description of architecture artifacts.
| | -   Learner will be able to explain how to transform collected architectural information and intents into viable models.
| | -   Learner will be able to depict functional requirements of the architecture.
| | -   Learner will be able to explain the vocabulary of their preferred Architecture Description Language (ADL).
| **CITA -- Specialist** | -   Learner will be able to conduct a threat modeling process
| | -   Learner will be able to apply some security methodologies, like OCTAVE, STRIDE, DREAD
| | -   Learner will be able to create architectures that are compliant to different standards from NIST, ISO, etc.
| | -   Learner will be able to implement a suitable security model.
| **CITA -- Professional** | -   Learner will be able to define and implement risk management in the enterprise
| | -   Learner will be able to implement and comply with security best practices indicated in know frameworks, like COBIT
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
| **CITA -- Specialist** | -   Learner will be able to conduct Protection Needs Elicitation procedures, like policy decomposition, data classification, misuse and abuse case modeling S-OM.
| | -   Learner will be able to identify the access control method to use in different cases
| **CITA -- Professional** | -   Learner will be able to identify, capture, manage, security requirements enterprise wide
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
| **CITA -- Specialist** | -   Learner will be able to implement technologies like identify management, certificate management, IDS, IPS, Virtualization, DRM
| | -   Learner will be able to identify issues and implement security adjustments for different types of architectures, like web applications, SaaS, RIA, pervasive computing, etc.
| | -   Learner will be able to perform an attack surface evaluation.
| **CITA -- Professional** | -   Learner will be able to evaluate the impact on business of each design decision and balance the cost benefit.

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
| **CITA -- Specialist** | -   Learner will be able to indicate the best development practices to be used during development.
| | -   Learner will be able to incorporate security during the corresponding development methodology
| **CITA -- Professional** | -   Learner will be able to evaluate the impact of vulnerabilities and solutions to strategy, and explain the long term impact to stakeholders.

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
| **CITA -- Specialist** | -   Learner will be able to explain the relation between software assurance an the acceptance criteria for pre and post deployment/release.
| | -   Learner will be able to understand what a software escrow is and why is needed.
| **CITA -- Professional** | -   Learner will be able to verify that the measures of the impact of the software to be deployed to the exiting computing ecosystems is being taken and analyzed.
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
| **CITA -- Specialist** | -   Learner will be able to define the requirements for the implementation of the incident management, patching and problem detection strategies.
| | -   Learner will be able to ensure the compliance with end-of-life (EOL) policies for software systems.
| | -   Learner will be able to ensure the hardening of software and hardware is in place and working as expected.
| **CITA -- Professional** | -   Learner will be able to explain why strategies for continuous monitoring, problem detection and incident management should be aligned to the business strategy and goal.
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
| **CITA -- Specialist** | -   Learner will be able to understand and apply the different regulations and acts in software architecture definition
| | -   Learner will be able to define an architecture the complies with AUP
| **CITA -- Professional** | -   Learner will be able to explain how regulations impact the business strategy and plan for a remedial solution
| | -   Learner will be able to measure the impact of regulations for globally used/distributed systems.

# Capabilities Resources

**Articles**

**Blogs/Webcasts/News Sources**

-   40 Security Blogs at [http://www.securityinnovationeurope.com/blog/40-information-security-blogs-you-should-be-reading](http://www.securityinnovationeurope.com/blog/40-information-security-blogs-you-should-be-reading){:target="_blank"}

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

