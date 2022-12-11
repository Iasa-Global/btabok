---
title: "Capacity Planning"
keywords: 
sidebar: mydoc_sidebar
toc: true
permalink: capacity_planning.html
folder: competency_model
summary: "The Capacity Planning architectural capability is going through a significant change at this time."
tags:
  - infrastructure_architecture
---

# Description 

Capacity is a key feature of any value delivering system. Failure to plan, design and oversee system capacity correctly can lead to the failure of the system to meet the needs of its stakeholders due to issues such as availability, performance or total cost of ownership.

As the capacity of any technology system is most often a function of the available infrastructure, capacity planning is most logically led by the infrastructure architect. The infrastructure architect must focus on meeting the needs of the system by understanding the business needs as defined directly by the system stakeholders or indirectly via interface and agreement with other architecture roles such as business, application data and solution architecture.

The Capacity Planning architectural capability is going through a significant change at this time. Up to relatively recently,  capacity planning focused more on making sure that adequate supply capacity was in place to meet forecast demand over a relatively long time horizon e.g. 3+ years. This often resulted in periods of oversupply, particularly early in the system's life. It also meant that, post implementation, capacity management was a reactive more than a proactive activity, driven by incidents rather than capacity monitoring. Where active capacity management was practiced the focus tended to be trying to identify when supply would no longer meet demand as early as possible to allow for slow moving upgrade cycles to complete.

Cloud based systems are turning capacity planning on its head. Real-time or near real-time supply models now mean that uncertainty on the demand side does not represent the same risk that the infrastructure architect had to cater for in the past. For architects designing solutions in the cloud, more emphasis on active capacity management is required, in particular ensuring that capacity can be scaled both up and down in line with dynamic demand patterns, thereby ensuring optimal system performance and cost. Gaining a deep understanding of demand aligns closely with the core capabilities of architecture but with that critical change of emphasis ­-- continuous as well as deep.

In this context the ITIL defined Capacity Management process in the Service Design phase is also a good source of guidance for architects of cloud solutions. In ITIL 3.0 the purpose of Capacity Management is defined as follows:

> [Capacity Management](http://wiki.en.it-processmaps.com/index.php/Capacity_Management#Business_Capacity_Management_ITIL){:target="_blank"} aims to ensure that the capacity of IT services and the IT infrastructure is able to deliver the agreed service level targets in a cost effective and timely manner. Capacity Management considers all resources required to deliver the IT service, and plans for short, medium and long term business requirements.

Doing architecture within the ITIL framework is one possible path to a more continuous form of architecture. For example, within ITIL, system requirements for capacity (demand) can be captured in a living contract -- the Service or Operating Level Agreement. This artefact can be actively maintained by service architects throughout the lifetime of the service, rather than potentially lost and forgotten by all active stakeholders in the solution requirements specifications from the original project. ITIL's focus on continuous service improvement may provide a valuable framework for architects accountable for capacity planning in a cloud based world.

# Overview

Capacity Planning is a foundation capability for all architects. Tied closely to the core pillar of Quality Attributes, the architect is responsible for ensuring that the capacity of any process, service or system meets the needs of all key system stakeholders e.g. investors, customers and consumers, not just on day 1 but throughout the full lifetime of the system.

## General Definition

The Wikipedia definition of [Capacity Planning](https://en.wikipedia.org/wiki/Capacity_planning){:target="_blank"}, taken from the [Supply Chain Resource Co-Operative](http://scm.ncsu.edu/scm-articles/article/capacity-planning){:target="_blank"}, while described in language more aligned to manufacturing, can also be applied to IT and IT systems/services. (As in many other areas, it is often good practice for IT architects to leverage approaches developed in other disciplines to advance the maturity of capacity planning and management in IT systems).

[**Capacity planning**](https://en.wikipedia.org/wiki/Capacity_planning){:target="_blank"}is the process of determining the production [capacity](https://en.wikipedia.org/wiki/Capacity_utilization){:target="_blank"} needed by an organization to meet changing [demands](https://en.wikipedia.org/wiki/Demand_curve){:target="_blank"} for its [products](https://en.wikipedia.org/wiki/Product_(business)){:target="_blank"}.[https://en.wikipedia.org/wiki/Capacity_planning#cite_note-NCSU-1](https://en.wikipedia.org/wiki/Capacity_planning#cite_note-NCSU-1){:target="_blank"} In the context of capacity planning, **Design Capacity** is the maximum amount of work that an organization is capable of completing in a given period. **Effective Capacity** is the maximum amount of work that an organization is capable of completing in a given period due to constraints such as quality problems, delays, material handling, etc. The phrase is also used in business computing as a synonym for [capacity management](https://en.wikipedia.org/wiki/Capacity_management){:target="_blank"}.

A discrepancy between the capacity of an organization and the demands of its customers results in inefficiency, either in under-utilized resources or unfulfilled customers. The goal of capacity planning is to minimize this discrepancy. Demand for an organization's capacity varies based on changes in production output, such as increasing or decreasing the production quantity of an existing product, or producing new products. Better utilization of existing capacity can be accomplished through improvements in [overall equipment effectiveness](https://en.wikipedia.org/wiki/Overall_equipment_effectiveness){:target="_blank"} (OEE). Capacity can be increased through introducing new techniques, equipment and materials, increasing the number of workers or machines, increasing the number of shifts, or acquiring additional production facilities.

As already suggested, combining a service oriented framework, such as ITIL, with concepts from other disciplines such as manufacturing will allow architects to design, plan and manage capacity more effectively.

## Capacity Planning Methods

A number of standard methods exist for capacity planning. The pros and cons or each are outlined in the following table:

| **Method** | **Description** | **Pros** | **Cons** |
| **Trending** | In trending, component behavior is modelled based on a simple linear model. | Relatively simple approach to implement. | May not reflect accurately real world non-linear impact on capacity. |
| **Simulation** | Simulation involves building a bespoke software based model that accurately mirrors the behavior of the real world system. | Flexible and potentially very accurate

Allows for significant levels of what-if analysis

 | The more complex the system the more expensive it will be to build an accurate model.

Requires specialist skills

 |
| **Testing** | The testing method uses a real-world copy of the system to carry out load analysis. | High levels of accuracy

Much less complex to build than simulation as should be replica of production environment

 | Cost -- accuracy based on degree to which test environment replicated production environment. |
| **Analytical Modelling** | Combines statistical analysis of real world data with a model that represents the complex interactions inherent in the system. | Potentially very accurate and allows for relatively inexpensive what-if analysis.

Uses relatively easily gathered data from real world system and does not require expensive test environments.

3^rd^ party tool support exists e.g. [Teamquest](http://www.teamquest.com/){:target="_blank"}, [VMWare Capacity Planner](http://www.vmware.com/products/capacity-planner/overview){:target="_blank"} etc.

 | As with simulation, analytical modelling requires end to end understanding of system -- business, application and technology. |

## Capacity Planning and Views & Viewpoints

While typically led by the infrastructure architect, all architects are responsible for carrying out Capacity Planning at their respective architectural layers e.g. enterprise, business, application, technology. In other words, capacity is an important Viewpoint [1](https://btabok.iasaglobal.org/btabok_3/capacity-planning/#_ftn1){:target="_blank"} that should be applied to all architectural Views[2](https://btabok.iasaglobal.org/btabok_3/capacity-planning/#_ftn2){:target="_blank"}.

## View Specific Capacity Planning

While the definition of standard views may vary by organization, for the purpose of this guide we will use the TOGAF defined views -- Business Architecture, Information Systems Architecture and Technology Architecture -- as an example of how the Capacity Viewpoint can be applied to each.

| **View Name** | **TOGAF 9.0 Definition** | **Capacity Planning Viewpoint** | **Examples** |
| --- | --- | --- | --- |
| **Business Architecture** | Business Architecture describes the product and/or service strategy, and the organizational, functional, process, information, and geographic aspects of the business environment. *[TOGAF 9.0](http://pubs.opengroup.org/architecture/togaf9-doc/arch/chap08.html){:target="_blank"}* | While significant automation may exist within a modern business process it is the number and behavior of the humans in the process that ultimately defines the load on the system.

In a non-dynamically managed system, clearly defined business process workflows are a critical input into the capacity planning process. In organizations where business processes are explicitly defined e.g. by a business architect, the maximum and average capacity of the business process should be estimated by the business architect.

Where a service oriented approach is used the business architecture should also identify all service components that play a part in the capacity of a system over an extended period. This viewpoint ensures that the capacity of supporting processes such as business management, monitoring, support and operations are also estimated.

 | The business architect of a Sales Order Taking process should provide both estimated maximum and average orders per hour and any longer term load trend factors such as market growth or seasonable fluctuations (based on customer demand estimates and number of resources allocated to process).

This capacity target can then be passed as a requirement to all impacted services/processes.

 |
| **Information Systems Architecture** | The Target Information Systems (Data and Application) Architecture, describes how the enterprise's Information Systems Architecture will enable the Business Architecture and the Architecture Vision, in a way that addresses the Request for Architecture Work and stakeholder concerns. *TOGAF 9.0.* | Typically the responsibility of the solution, data and/or application architect, business/service capacity requirements must be gathered and translated into specific requirements for logical data and logical application architectures.

The application architect should ensure that the logical application technology architecture can meet these requirements either directly via dedicated application components configured with the required capacity or indirectly via shared infrastructure components -- typically agreed with the infrastructure architect/infrastructure solution architects.

 | In applications requiring highly scalable capacity logical application design patterns that are based on stateless, message based application servers connecting to a distributed, in-memory database may be appropriate, as this will allow the most flexibility in terms of meeting dynamic capacity requirements.

Systems that have a more fixed capacity requirements may be better served by a simpler application architecture that does not require complex or specialized supporting components.

 |
| **Technology Architecture** | The Technology Architecture enables the logical and physical application and data components and the Architecture Vision, addressing the Request for Architecture Work and stakeholder concerns. *TOGAF 9.0* | Solution or infrastructure architects must gather requirements from application/data architects and translate them into the required technology architecture.

Depending on the size, scale and complexity of the system, infrastructure components can be relatively simple e.g. local server CPUs/disks/memory/network links or relatively complex e.g. shared infrastructure services such virtual server farms, storage area networks, load balanced geo-stretched VLANs.

In the lowest architectural layer, physical environment, infrastructure architects must also ensure that adequate aggregate capacity is in place in terms of data center floor space, racking, power, air conditioning and cabling.

Infrastructure architects responsible for cloud type systems must also be able to put in place tools and processes to allow for dynamic capacity management. E.g. Amazon AWS and Microsoft Azure IAAS and PAAS services use service wrappers and automated service provisioning and management tools.

 | At this level architects can choose between a range of infrastructure design patterns that can provide different capacity options at different price and performance points including:

-   proprietary (Windows, UNIX, VMWare) or open source (LINUX, OpenStack) platforms
-   on-premise or cloud based solutions
-   fixed or dynamic capacity management tools

 |

## Capacity Planning and Managing architectural accountability

Closely related to View and Viewpoints, it is critical that the infrastructure architect manages relationships with all dependent layers, either directly or indirectly, through some form of formally managed agreements. In practice, accountability for Capacity Planning is often split between a number of different but highly interdependent architecture roles e.g. enterprise, business, application, data, solution, service and infrastructure. Ensuring accountability is clearly defined at each level is critical to ensure that long term, end to end system capacity meets business requirements. In practice this can be difficult to achieve for a number of reasons:

-   Traditionally architects have not been involved in the day to day running of a system and therefore changes that are a result of increased load are not always tracked against the original capacity design leading to capacity related issues that are perceived as an IT service delivery issue rather than a known capacity constraint that is linked to the original design and associated capital investment.
-   In large enterprise systems, tracking change through the different architectural layers is complex and difficult to achieve. Changes at one level may be difficult to communicate clearly at all architectural levels. This can make root cause analysis complex and as a result capacity related issues are not always identified correctly as such.

One approach to tackling this challenge is to ensure that where architectural accountability switches from one architect to another, a formal agreement of some sort is put in place that captures clear capacity related terms and conditions. Examples of such formal operating agreements are Service and Operating Level Agreements as defined in ITIL or [standardized service contracts](https://en.wikipedia.org/wiki/Standardized_service_contract){:target="_blank"} as defined in SOA.  The architect's role is typically to create these contracts and hand over to the service management team to monitor and manage. Architectural involvement is also recommended when and where these contracts need to be renegotiated.

## Capacity Planning, Platforms and SDLC Approaches

The nature of the target infrastructure platform is a critical factor when designing the optimum approach to Capacity Planning. In environments with more traditional models of on-premise infrastructure, a waterfall based approach may be most appropriate. In this approach a detailed theoretical design is completed based on a detailed assessment of demand (short, medium and long term) against availability risks i.e. risk that capacity may unpredictably spike beyond available levels, lead time of provisioning additional capacity and analysis of costs associated with provisioning capacity at different times in the lifecycle of the service. This design is then tested using simulated load, where an appropriate test environment is available. While a valid approach the resulting system's capacity is largely fixed with major capital investment required up front and can only be increased (or decreased) as part of a major and often expensive change project.

Where more agile approaches are adopted, more dynamic approaches to capacity planning and design are required. This puts a much greater emphasis on a system design that supports dynamic capacity management as a key system attribute.

Well-designed cloud systems -- public or private -- should always support this approach. In these systems the focus of capacity planning moves from design and testing using simulated load to gathering real time data on the performance of the system at different levels of actual load and using this data to:

1.  Automatically provision additional shared capacity and

Carry out some form of analytical modelling to identify capacity related trends and allow for timely capital investments to add additional capacity.

*Iasa BTABoK:* A ***viewpoint*** defines the perspective from which a view is taken. More specifically, a viewpoint defines: how to construct and use a view (by means of an appropriate schema or template); the information that should appear in the view; the modeling techniques for expressing and analyzing the information; and a rationale for these choices (e.g., by describing the purpose and intended audience of the view).

*Iasa BTABoK:* A **view** is a representation of one or more structural aspects of an architecture that illustrates how the architecture addresses one or more concerns held by one or more of its stakeholders.

# Proven Practices

For an architect Capacity Planning can be broken into the following practices:

| **Practice** | **Description** | **Approaches/Methods/Patterns** |
| --- | --- | --- |
| **Determine & Agree Capacity Requirements** | Estimating and designing the capacity of a complex system requires a detailed understanding of all system elements and the complex interactions that are driven by the in scope business processes through application and infrastructure layers.

In modern complex systems requirements must be traceable between each layer. Business architects define the business processes and associated capacity requirements. These requirements are then handed to the application architects who design the application architecture to meet the business process requirements. Lastly, the application architects provide capacity requirements to the infrastructure architects for CPU, memory, storage and networking design.

To ensure maximum traceability a system of formal agreements/contracts between architectural layers is recommended, in particular where accountability switches between different architects.

*Waterfall Approach*

In a traditional waterfall approach capacity requirements are captured during each main design phase -- business case, high-level design and detailed design in a range of artefacts such as business cases, PID's, functional specifications etc.

*Agile Approach*

In an agile approach, short term capacity requirements are gathered only, allowing for quicker and less expensive system implementation. This approach works best for systems with less predictable and more variable capacity requirements. While still evolving the DevOps community are developing capacity planning and management processes that are appropriate for agile implementations.

*Service Oriented Approach*

Where a service oriented approach is used (can be applied to both waterfall and agile), capacity requirements can be captured in service and operating level agreements.

 |
| **Baseline Current Capacity** | Unless working on a greenfield design i.e. no current capacity, gaining an understanding of the current system capacity is a critical step in capacity planning.

To complete this activity two key activities must be completed:

1.  Current Configuration

Inventory of current system configuration at each architectural view. For example business architects should understand nature of allocated human resources. Application architects should provide an inventory of all application components in the context of the business processes they automate. Solution and infrastructure architects should provide details of allocated compute, storage, network and data center resources.

1.  Historical Load

Detailed data on historical load is also required at all levels and for all components.

 | Different approaches to baselining current capacity are typically required depending on the organization's process maturity.

-   Low Maturity

Baseline current capacity through standard data gathering approaches such as documentation reviews, workshops and leverage available automated system discovery and monitoring tools.

-   Average Maturity

Leverage configuration management systems to baseline configuration and monitoring systems to evaluate load history.

-   Leading Maturity

Leverage active and up to date system capacity reports that are maintained as part of standard operating procedures.

 |
| **Design Capacity** | Architects must understand common architectural patterns for capacity design and select the optimum pattern i.e. highest return on investment, for the specific business requirements.

Capacity design patterns continue to evolve rapidly from static, on-premise, capital intensive patterns to dynamic, public cloud, opex intensive patterns and everything in between.

Given the inherent elasticity of cloud solutions the emphasis in capacity design moves meeting long term requirements to a more dynamic capacity planning approach. This requires much more focus on end to end infrastructure service management including usage based charge-back mechanisms.

Architects need to understand how different levers, in particular price, can be used to manage capacity and maintain the right balance between demand and supply.

 | *On-Premise -- Static Capacity -- Capex Intensive*

Traditional approach based on building for medium to long term capacity requirements. Adding significant additional capacity typically requiring major additional capital investment.

*On-Premise  -- Dynamic Capacity -- Capex + Opex Intensive Approach*

Private cloud approach. Designed for more flexible capacity management using advanced tooling. Requires higher levels of ongoing system management.

*Public Cloud -- Extensive Dynamic Capacity -- Opex Intensive*

Public cloud approach. Designed for maximum capacity flexibility. Opex oriented model may be more expensive over longer time horizon.

 |
| **Manage Capacity** | The need for an architect to proactively manage the capacity of a system is increasing. Where traditionally the architects active involvement ended once an initial system design and build phase is completed and handed over to operations/service management, business requirements for greater flexibility and agility are increasing the need for architects to move to a more continuous and proactive role in capacity management. This is particularly true where public cloud solutions are used, for example, to ensure that longer term opex costs are correctly understood by the business. | On-Premise Approach

In traditional on-premise hosting approaches the capacity (largely fixed), of a system is typically agreed by the architecture team with the customer during the design phase. The system is then built to the agreed design and enters operation. At some point in the future service incidents/problems may be identified that have capacity as the true root cause but in many cases is perceived by the service consumers as an IT issue. In this case it is the architect's responsibility (at original handover point if necessary) to ensure that service management teams have a clear understanding of the agreed capacity and ensure that this is monitored and reported on regularly.

Cloud Approach

Reflecting the dynamic nature of capacity management in a cloud service it is critical that service demand and service supply are managed in real-time. The architect must design appropriate request management, provisioning, monitoring and reporting systems that proactively manage system capacity and avoid capacity related service outages and incidents.

 |

# Sub-Capabilities

## Determine & Agree Capacity Requirements

| **Iasa Certification Level** | **Learning Objective** |
| **CITA -- Foundation** | -- Learner will be able to describe general approach to gathering and agreeing capacity requirements.
| | -- Learner will be able to name some of the different approaches to capacity requirements gathering e.g. waterfall, agile.
| **CITA -- Associate** | -- Learner will be able to describe the differences between various approaches to gathering and agreeing capacity requirements.
| | -- Learner will be able to describe the key elements of capacity requirements analysis as practiced by architects in different domains.
| **CITA -- Specialist** | -- Learner will be able to describe when it is most appropriate to use different capacity requirements gathering and agreement approaches, and highlight the advantages and disadvantages of each
| |-- Learner will be able to describe how to use at least one of the approaches in detail for a project and be able to produce examples of their work
| **CITA -- Professional** | -- Learner will be able to identify new approaches for different groups of stakeholders
| | -- Learner will know the risk of not completing all aspects of gathering and agreeing capacity requirements and be able to justify this where appropriate


## Baseline Current Capacity

| **Iasa Certification Level** | **Learning Objective** |
| **CITA -- Foundation** | -- Learner will be able to describe general approach to baselining current capacity of target service, process, application, system.|
| |-- Learner will be able to name some of the different approaches to baselining current capacity.
| **CITA -- Associate** | -- Learner will be able to describe the differences between various approaches to capacity baselining.
| | -- Learner will be able to describe the key elements of current capacity baselining as practiced by architects in different domains.
| **CITA -- Specialist** | -- Learner will be able to describe when it is most appropriate to use different current capacity baselining approaches, and highlight the advantages and disadvantages of each
| | -- Learner will be able to describe how to use at least one of the approaches in detail for a project and be able to produce examples of their work
| **CITA -- Professional** | -- Learner will be able to identify new approaches for different groups of stakeholders
| | -- Learner will know the risk of not completing all aspects of current capacity baselining and be able to justify this where appropriate


## Design Capacity

| **Iasa Certification Level** | **Learning Objective** |
| **CITA -- Foundation** | -- Learner will be able to describe general approach to capacity design of target service, process, application, system.
| | -- Learner will be able to name some of the different approaches to capacity design.
| **CITA -- Associate** | -- Learner will be able to describe the differences between various approaches to capacity design.
| | -- Learner will be able to describe the key elements of current capacity design as practiced by architects in different domains.
| **CITA -- Specialist** | -- Learner will be able to describe when it is most appropriate to use different current capacity design patterns, and highlight the advantages and disadvantages of each
| |-- Learner will be able to describe how to use at least one of the design patterns in detail for a project and be able to produce examples of their work
| **CITA -- Professional** | -- Learner will be able to identify new design patterns for different types of stakeholder needs.
| | -- Learner will know the risk of not completing all aspects of capacity design and be able to justify this where appropriate

## Manage Capacity

| **Iasa Certification Level** | **Learning Objective** |
| **CITA -- Foundation** | -- Learner will be able to describe general approach to managing capacity of target service, process, application, system.
| |-- Learner will be able to name some of the different approaches to capacity management.
| **CITA -- Associate** | -- Learner will be able to describe the differences between various approaches to capacity management.
| |-- Learner will be able to describe the key elements of capacity management as practiced by architects in different domains.
| **CITA -- Specialist** | -- Learner will be able to describe when it is most appropriate to use different current capacity management approaches, and highlight the advantages and disadvantages of each
| |-- Learner will be able to describe how to use at least one of the approaches in detail for a project and be able to produce examples of their work
| **CITA -- Professional** | -- Learner will be able to identify new approaches for different types of stakeholder needs.
| | -- Learner will know the risk of not completing all aspects of capacity management and be able to justify this where appropriate

# Related Capabilities

-   [BTS -- Requirements Discovery and Constraints Analysis](requirements_discovery_and_constraints_analysis.md){:target="_blank"}
-   [HD -- Collaboration & Negotiation](collaboration_and_negotiation.md){:target="_blank"}
-   [DES -- Requirements Modeling](requirements_modeling.md){:target="_blank"}
-   [DES -- Whole System Design](the_whole_systems_design.md){:target="_blank"}
-   [DES -- Traceability throughout the Lifecycle](traceability_throughout_the_lifecycle.md){:target="_blank"}
-   [DES -- Views & Viewpoints](https://btabok.iasaglobal.org/btabok_3/capability-descriptions/views-and-viewpoints/){:target="_blank"}
-   [ITE -- Change Management](https://btabok.iasaglobal.org/btabok_3/change-management/){:target="_blank"}
-   [ITE -- Infrastructure](https://btabok.iasaglobal.org/btabok_3/capability-descriptions/infrastructure/){:target="_blank"}
-   [ITE -- Testing, Methods, Tools and Techniques](https://btabok.iasaglobal.org/btabok_3/testing-methods-tools-and-techniques/){:target="_blank"}
-   [QA -- All Capabilities](competency_model_m.md){:target="_blank"}

# Resources


**Articles:**

[Capacity Planning (Wikipedia)](https://en.wikipedia.org/wiki/Capacity_planning){:target="_blank"}

[Capacity planning isn't dead, but it's not about supply any more](http://devops.com/2014/10/28/capacity-planning-isnt-dead-supply/){:target="_blank"}

**Blogs/Webcasts/News/Reference Resources:**

IVI IT-CMF -- Capacity Forecasting & Planning Capability -- [http://ivi.nuim.ie/it-cmf/capacity-forecasting-and-planning](http://ivi.nuim.ie/it-cmf/capacity-forecasting-and-planning){:target="_blank"}

IVI IT-CMF -- Demand & Supply Management -- [http://ivi.nuim.ie/it-cmf/demand-and-supply-management](http://ivi.nuim.ie/it-cmf/demand-and-supply-management){:target="_blank"}

The Open Group web site: [http://www.opengroup.org/subjectareas/enterprise](http://www.opengroup.org/subjectareas/enterprise){:target="_blank"}

TOGAF: [http://pubs.opengroup.org/architecture/togaf9-doc/arch/index.html](http://pubs.opengroup.org/architecture/togaf9-doc/arch/index.html){:target="_blank"}

ITIL: [http://wiki.en.it-processmaps.com/index.php/Capacity_Management#Business_Capacity_Management_ITIL](http://wiki.en.it-processmaps.com/index.php/Capacity_Management#Business_Capacity_Management_ITIL){:target="_blank"}

CMIS: [http://www.teamquest.com/import/pdfs/whitepaper/capacity-management-information-system.pdf](http://www.teamquest.com/import/pdfs/whitepaper/capacity-management-information-system.pdf){:target="_blank"}

How to do capacity planning: [https://www.youtube.com/watch?v=w0cD26CLBA0](https://www.youtube.com/watch?v=w0cD26CLBA0){:target="_blank"}

# Author

![Paddy Baxter](media/p_baxter.jpg)
**Paddy Baxter**
*IT Architect*

Paddy's natural strengths of intuitive, big picture analysis, combined with a strong desire to improve on existing systems for the benefits of all stakeholders, have led him to the profession of enterprise architecture. Paddy has over 25 years' experience in large enterprise IT environments across the globe, working in Europe, Australia, Asia and the US with major industry players such as HP (Digital/Compaq), Microsoft, Intel and EY.

Most recently Paddy has worked with a number of major client in life sciences, utilities and banking in areas such as mobile, SAAS adoption and operating model design. Paddy is currently working with clients in Ireland to help them mature their architecture capabilities and through this help them to transform to survive and ultimately thrive on the tidal wave that is digital disruption.

