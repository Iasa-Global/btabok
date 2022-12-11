---
title: "Device Management"
keywords: 
sidebar: mydoc_sidebar
toc: true
permalink: device_management.html
folder: competency_model
summary: "The policies that are in place around the use of these devices is determine by requirements that are needed to support the specified device use scenarios."
tags:
  - infrastructure_architecture
---

# Description

Devices are assets that are IT infrastructure endpoints. They typically contain, data, software and sensors and/or actuators to enable the IT environment to interact with the external environment.

These Devices having varying degrees of connectivity, intelligence and security that need to be factored into the set of architectural choices that are adopted.  Device management is essential and is required to perform many device management tasks:

-   Provisioning includes initialization and activation of devices
-   Configuration includes establishment of setting and parameters for device operation.
-   Software upgrade are required to improve device operating mode, performance and potentially security.
-   Fault management is required to deal with error reporting and device status updates. This area also includes capability to deal with device faults and extraordinary behaviours.

Devices themselves are deployed in a range of configurations that include:

-   Direct connection to another device. ( a simple case of Machine 2 Machine or M2M)
-   Connection to another device through a limited range network (M2M)
-   Connection through a gateway or over the Internet (Internet of Things)

Connection through a mobile device (either with Internet or through proprietary communications network --Mobile Device).

# Overview

The policies that are in place around the use of these devices is determine by requirements that are needed to support the specified device use scenarios.   Clearly, the underlying architecture and policies that are needed to support something like a mobile phone differs substantially from the architecture that is needed to support a real-time embedded device.

Based on business requirements the architect needs to provide direction on the management policies that deal with items such as:

**Device Connectivity** to the infrastructure.   How does the device exploit the network to connect with the infrastructure?  Is the device domain joined? What are the protocols that are required to support the bandwidth requirements?  E.g. Mobile devices have very different needs than embedded devices in terms of both bandwidth and security.  The device connectivity needs to be examined to determine the best means to achieve device management given network features (including network bandwidth, performance and latency restrictions) versus the level of autonomy the device has. In some case, multiple network may become necessary to separate device management from real-time data passing.

**Device Data Content** and Privacy need to be managed.   Is the data that resides on the device secure?  What network protocols are used to authentic and ensure the privacy of device information. Also for actuators working on stuff like the Internet of Things how do we prevent cyber-attacks on our devices?

**Device Software** needs to be managed to ensure it provides for the end point needs.  Lifecycle management is just one aspect.  What sorts of experience and information does this software provide? What patterns are applied to interact with the main infrastructure? Real time telemetry would be structured quite differently than mobile phone Office software.

**Device Reporting** is a facet of device management that allows for reporting on the current device state.

**Device Identity and Security** also need to be managed and also in a way to clearly support identity authentication, authorization, auditing and administration requirements.

Separation of user versus corporate information has become a significant trend with consumerization and bring your own device work policies.

Devices management is usually in the context of reference models and networks.

## Why Does an Architect need this Skill?

Device management is based on careful consideration of the device use scenario and working quality attributes and their trade-offs with various designs around those scenarios. As devices vary according to intelligence, band-width requirements, form factor, connectedness etc.  So to the policies that manage that device need to be established and managed across the areas identified.

Having the proper knowledge and understanding of the different aspects of device management will allow the architect to articulate the importance and the need for such an exercise both on a tactical and a strategic level.  In addition, they will help ensure the development of device management policies that supports the technology and enterprise architecture standards of the Enterprise.   IN addition these policies are managed through service management processes ( such as ITIL or MOF) in a more mature enterprise so the architect needs to understand how these configuration services are used to manage device policies as part of the overall architecture.

Various standards bodies have already established some of the fundamental protocols and reference architectures that need to be considered to ensure that devices are appropriately managed.  In addition there are unique quality attributes that need to be considered (such as situations where the devices are limited by lower power consumption, autonomy requirements etc.) Several M2M and IoT architectures that have been proposed include:

-   European Telecommunications Standards Institute M2M / one M2M (ETM)
-   International Telecommunication Union -- Telecommunication Sector (ITU-T)
-   Internet Engineering Task Force (in progress)

Mobile Devices are currently managed through proprietary architectures (Microsoft, Citrix, Good, Air Watch etc.)  and more open models such as the one proposed by Gartner.    In addition consortiums will soon be releasing more standardized reference models and architectures for all the device management modalities (M2M, IoT, Mobile etc.).

## Common Tasks Involved with This Skill

The architect will be involved in multiple phases of Device Policy Management.

-   Assist in creating a requirements document by consulting with various technical, business stockholders and lines of business and identifying device use scenarios. The architect should review the requirements for feasibility and value proposition. For example, telemetry small form factor devices may require more succinct data sharing protocols than a mobile phone.
-   The architect will assist in defining risk profile for the enterprise related to the use and connection of the devices to the corporate infrastructure.
-   The architect need to ensure that the device conforms to the overall technology standards of the infrastructure.
-   The architect has to ensure the design address device availability, performance, use in lower power and limited network setting -- other quality attributes related to the function of that device in designated scenarios need to be considered. The level of device autonomy and intelligence also need to be considered.
-   Architect to involve engineering and operations team in the architectural design to ensure effective and agreed on solution across the design, build and run technology stack.
-   Create a set of device policies that provide data, software, privacy and identity management.
-   Assist through the deployment phase of the project, during this step the engineering team will deploy the solution as per design document. The architect should monitor and evaluate the deployment to ensure that it meets defined design and modify procedure or architecture if deemed necessary.
-   The architect need to ensure that the design document is included as part of the project/initiative artifacts. Such information should be readily available for reference by various engineering groups.
-   Familiarity with ITIL is needed to support configuration management activities around device management.

## What is Their Ownership in this Skill?

The architect(s) will lead the architectural aspect of device management, as well as guiding the organization with vendor selection and negotiation. In larger organizations there might be multiple architects with different areas of expertise involved in setting these device policies.  For example, a network architect may be involved in helping to work with network bandwidth issues for device usage along with setting actual policies on device usage based on the requirements.

Often devices will operate under unique network conditions.  In addition Device management based solutions are part of larger device architectures and will need to address relevant operation of gateways, networks (ranging from Internet, specialty networks, propriety telecommunications networks etc.)

## How is this skill used by the architect in daily activities?

The Architect would be expected to be able to:

-   Understand the requirements to build a viable network design.
-   Understand both physical and logical requirements to achieve desired architecture.
-   Present solution to management and other stakeholders.
-   Understand different technology offerings in the market place, understanding technology landscape will allow the architect ability to design and/or recommend appropriate solution(s).
-   Ability to translate business requirement to technical design.
-   Ability to explain complex technical design in a way that non-technical people may understand.
-   Knowledge of total cost of ownership modeling as it pertains to IT investments
-   Provide guidance on the management of these policies in the context of configuration management processes and service processes such as ITIL.

Understand whole system design and how to make quality attribute trade-offs within the infrastructure.

# Proven Practices

## Describe why an architect should be involved in this skill at a corporate level.

An architect is responsible for linking technology decisions with business strategy. It is increasingly evident that technology and the business cannot operate independently and there is a paradigm shift from perceiving IT as a cost center to IT as a business enabler. Solution or enterprise architect is uniquely positioned to bridge the gap between business requirements and technical reality.

# Sub-Capabilities

| **Iasa Certification Level** | **Learning Objective** |
| :-: | :-: |
| **CITA- Foundation** | -   The Learner should be able to identify the key scenarios and recognize how these requirements match with various devious policies.
| | -   The learner should be able to describe the different device types that require policy management as well as the nature of those policies.
| | -   The learner should be aware of the basic device architectures and models as defined.
| **CITA -- Associate** | -   The Associate is able to articulate the key considerations in the design including Device management trade-offs between bandwidth and device intelligence /autonomy.
| | -   The associate must be able to differentiate between different scenario to describe how different policies impact quality attribute trade-offs inherent in those scenarios.
| | -   The associate needs to understand how device management policies relate to configuration Management.
| | -   The associate should be able to use an appropriate reference model to match a given set of user scenarios.
| **CITA -- Specialist** | -   The specialist is able to discuss the architectural implications various kinds of devices that includes mobile data management, embedded devices etc.
| | -   The specialist is able to describe how to manage these device policies and formulate complex policies from overall design considerations.
| | -   The specialist is able to articulate cost implication of the defined design. Also the ability to articulate cost/benefit analysis based on various solution options.
| | -   The specialist is able to customize areas of the design to meet unique scenarios.
| **CITA -- Professional** | -   The professional will have experience with delivering architectural programs leveraging complex environments and can discuss working with engineering and operational teams.
| | -   The professional has an ability to change their device management policies based on further discussion with different stakeholders and explain in detail all the aspects required in making trade-off in the architecture based on requirements and how they impact quality attributes.
| | -   The professional will understand different approaches to manage devices in modalities such as IoT and mobile device management.
| | -   The professional will be able to articulate the impact of decisions from different layers in the device architecture have on their management.

# Resources

Wikipedia Mobile device management overview: [http://en.wikipedia.org/wiki/Mobile_device_management](http://en.wikipedia.org/wiki/Mobile_device_management){:target="_blank"}

Wikipedia embedded device management overview (Internet of Things): [http://en.wikipedia.org/wiki/Internet_of_Things](http://en.wikipedia.org/wiki/Internet_of_Things){:target="_blank"}

Embedded Device Management with System Center

[https://msdn.microsoft.com/en-us/library/ff769910(v=winembedded.60).aspx](https://msdn.microsoft.com/en-us/library/ff769910(v=winembedded.60).aspx){:target="_blank"}

Mobile Device Management with System Center:

[https://technet.microsoft.com/en-us/magazine/hh316170.aspx\](https://technet.microsoft.com/en-us/magazine/hh316170.aspx/){:target="_blank"}

**Other References:**

From Machine-To-machine to the Internet of Things by Jan holler ET. Al.

Smart Stuff an Introduction to the Internet of Things, b David W. Stephenson.

Mobile Device Management by Patrick Finch

# Author

![Farzad Ahmed](media/b_ominski.jpg)
**Brice Ominski**
*ITAP Consultant -- Microsoft*

Provides thought leadership and practical trusted advice that enables business strategy through technology to C-level and senior management. He is an Information Technology and Architecture Planning (ITAP) advisor for Microsoft who successfully translates business strategy and requirements to propose, develop and implement Enterprise level solutions to meet overall business objectives and manage risk. Recently obtained IASA CITA-P certification.

