---
title: "Risk Methods"
keywords: 
sidebar: mydoc_sidebar
toc: true
permalink: risk_methods.html
folder: engagement_model
summary: "Managing risk is an important aspect of delivering an architecture and influences the decision-making process."
tags: 
  - value_model
---
> "The possibility of something bad happening at some time in the future; a situation that could be dangerous or have a bad result." 
**definition of Risk, Oxford Dictionary**

# What is Risk

Almost any business venture or action carries possibility of potentially negative effects. In fact, people face risks every day in our lives, the risk of being run over when crossing the street, the risk of falling of a ladder, the risk of losing money on an investment. In many of these everyday cases people often may not even realize that they are making judgments and taking decisions to manage risks, it kind of happens automatically.

A risk is something which, if realized, has outcome which results in negative consequences [to an entity such as an organization or an individual]. The good thing about risks is that they are identified before the outcome, and this provides an opportunity to take action against the risk and limit its impact.

Working with architecture is no different to other business activities, and it is particularly important to identify risks in a timely fashion and address the risks with appropriate actions.

The following three important aspects of a risk will help the architect in establishing the priority and significance of the risk.

-   **Probability** -- the likelihood that the risk will be realized
-   **Consequence** -- the seriousness of the consequences if the risk is realized
-   **Mitigation** -- that which can be done to reduce the probability or consequences of the risk

Managing risk is an important aspect of delivering an architecture and influences the decision-making process.  Note that this section of the BTABoK does not attempt to exhaustively define risk terminology (if you are unfamiliar with Governance, Risk and Compliance terminology it is recommended that you get a basic grounding in this area -- see the references section) instead it highlights key risk methods as they relate to Architecture.

Its important to note that a risk that has been realized ceases to be a risk, it becomes an actual issue or problem.

# Why do we need to Manage Risk

Since risks influence the decisions made when developing an architecture it is important that risks are identified and managed. Being aware of risks helps the architect to make the right decisions when faced with several alternative solutions.

Identifying and managing risks allows the architect to foresee consequences and act accordingly to mitigate negative effects.

Many risks involve several stakeholders, who will have to collaborate to mitigate such risks. It is important that the architect manages and communicates risks to other stakeholders since this can reveal unseen consequences and even opportunities.

It may be the case, that it is extremely difficult to mitigate some risks, especially if they are the result of actions external to the organization. For example, changes in law, government or regulation. However, it is important that the architect and the organization are aware of these risks and plan for the consequences, should the risk be realized.

Risks affect strategy and tactics, which in turn affect the architecture. What was once an acceptable risk can quickly change to an unacceptable risk. This may result in a change of tactics or strategy which has a significant effect on the architecture. For example, changing standard technologies, changing platform suppliers, or moving the focus for product features.

Without the management of risk, these negative effects can appear spontaneously with no fore-warning. This put unnecessary stress on the organization and architect to react quickly find solutions under pressure, which in turn can lead to mistakes and sub-optimal solutions. Risk management provides the ability to reduce the impact of negative effects and plan ahead to avoid such situations.

# Risk Approach

## Role of the Architect

If the choices or implementation results in significant technical debt these should be recorded (ideally on a risk register if the organization has one). The architect is often called upon to translate the nature of an architectural or technical risk into terminology business stakeholders (in particular risk owners) can understand so that they can make informed choices about risks. A good example of this is in cybersecurity -- where the risk landscape is highly technical and specialized.

## Visibility of Enterprise / Solution Risks is crucial

In order for architects to align their work with considerations around significant risks it is important to get visibility of them. Where are risks identified and managed strategically within the organization (or for the relevant product / platform / project?) In highly regulated organizations or where there is a high level of risk management maturity this can be more straightforward. There will be a risk register and management accountability for risk management (often a Chief Risk Officer and/or Governance Risk and Compliance teams). In other organizations risk is far more federated within other roles and in some cases isn't explicitly called out -- it might sit within legal or compliance or business unit leadership.

Whatever the approach to risk within the organization its key to understand where risk management activities are taking place so that architecture can be risk aligned (or where appropriate risk driven -- if risk reduction is the primary objective). Some improvement of the maturity of risk management may be required (and this in itself can be argued to be an enterprise or business architecture activity).

## Balance Risks with Benefits

As stated earlier risks are all around us and organizations take calculated risks in order to operate, differentiate and achieve their strategic goals. As an example financial services firms decided to offer internet based banking in order to retain and attract customers -- despite the significantly increased risks. The vast majority of global banks have decided the benefits outweigh the risks and so offer internet and mobile based banking.

# Risk Management

In order to reduce the impact or remove risks, they need to managed and monitored throughout the development of the architecture. Many of the risk management processes and techniques which are used in business and project management can be applied to managing risks in the development of an architecture both at enterprise and solution level.

## Types of Risk

The context of the assignment generally defines the types of risk which have to be dealt with. The following are a number of examples of risk types which can be considered when working with architecture (note that this is not exhaustive and the relevance of different risk types will of course vary depending on the nature and industry vertical of the organization).

## Technology

Technology risks are perhaps the first type which jumps to mind when working with an architecture. These types of risks can be associated with technology decisions on the architecture, for example, selecting platforms, development tools or architectural styles. A typical example of a technology risk would be employing a cutting-edge technology as a basis for the architecture, while this may give significant gains in development time, this is a risk that the technology will not gain traction on the market. This can result in serious long-term maintenance problems.

## Financial

The implementation of an architecture needs to be funded, and the decisions made when developing the architecture affect the cost of the resulting implementation. Financial stability is a significant factor in getting an architecture to implementation. Certain architecture decisions can present a risk of exceeding the assignment budget, the consequences of such risks can vary depending on how stringent the budget is. Different assignments in an organization will also be competing for fincances, the risk of losing finances to assignments with a higher priority should be taken into consideration.

## Organization

Organization is an important consideration when developing the architecture to ensure that the architecture is feasible for implementation. The organizational structures and processes have to be in place in order for the architecture to succeed, but these often develop along-side the architecture. There may be risks in the areas personnel skills, capacity, or under-developed capabilities. Partnerships with other organizations, both internal and external, create dependencies where risks should be assessed.

## Legal and Regulatory

Changes in law or regulatory requirements can represent a risk for the architecture. Such changes can affect designs or add significant new requirements changing the quality attributes of the architecture. The legal requirements on the architecture may be different for different countries, so consideration has to be given to risks, especially if a product is being deployed globally. A typical example this is the potential introduction of new privacy laws in several countries. It is important to monitor the risk of legal or regulatory change since these can have a severe effect on delivery of products or services based on the architecture.

## Political

Internal and external politics can present risks for the implementation and delivery of architecture. Internal politics affect the architecture, since stakeholders which the architecture depends on can block or make delivery difficult, depending on their interest. This can be seen when working with technologies which will replace existing technologies. The stakeholders in the existing technology may not accept the new technology for political reasons, and this represents a risk. Decisions in the architecture development affect the political risk.

External politics can also effect the architecture where a change in government policies can lead to potential changes legal or regulatory requirements, leading to risks.

## Qualitative Risk Assessment

Qualitative risk assessment is a subjective method of assessing risks. It uses the probability and consequences (sometimes called impact or severity) of the risk to create a ranking. The ranking for risks is often high, medium or low. This helps when performing a risk assessment to prioritize risks for mitigation, for example, mitigating high risks first. A typical method for performing a qualitative risk assessment is to use a risk matrix.

The qualitative method is often based on the experience of the participants and is quick and inexpensive, however, it lacks the accuracy that can be gained by using quantitative methods.

## Quantitative Risk Assessment

Assessment of risks based on financial impact or other metric.

## Tackling Risks ("Risk Treatment")

Once a risk has been identified it then needs to be assessed and treated -- generally in one of the following ways. The alternative can be thought of as a kind of anti-pattern akin to risk ignorance.

-   Avoidance
-   Reduction (or Mitigation)
-   Sharing and Transferring
-   Acceptance

## Avoidance

Choosing to actively avoid the risk. In many cases when it comes to technology transformation this isn't a practical option. Avoidance has consequences. In this example avoiding the security, legal and data jurisdiction risks of a cloud based architecture means you are accepting the consequence of maintaining your own infrastructure.

## Reduction (or Mitigation)

Reduction or mitigation of a risk means finding ways to lessen the impact or effect of the risk. This results in less severe consequences. For example, if there a risks and uncertainties regarding the security of an architecture, these may be mitigated by performing actions such as threat analysis, information classification and penetration testing.

## Sharing and Transferring

It may be possible to transfer a risk or share a risk with another party such as a supplier, partner or insurance company. This provides a way to either remove the consequences of the risk or significantly lessen the impact of the consequences. For example, there may be a risk to providing the required availability of a given service, perhaps appropriate operational skills are hard to find. It would be possible to move this risk to a partner company that takes responsibility for operation and availability of the service.

## Acceptance

Acceptance of a risk means that the organization is willing to deal with the consequences of the risk as-is. This is perhaps a trade-off in a particular decision where the benefits of the decision out-weight the probability of the negative consequences of the risk being realized. It may even be that the negative consequences are acceptable against the value gained. For example, there may be a risk performing a product release with poor scalability, the negative costs to scale the product may be off-set against getting the product to market before competitors.

# Quality Attributes and Risk

Quality Attributes (including non-functional requirements) are critical yet often overlooked or deprioritized by business stakeholders. Focusing on features, time to market and pressures to keep costs minimal lead to risks that solutions do not align with the required level of quality. Architects can reduce the risk of these being overlooked by making them explicit -- calling out what the impact and risk of corner cutting can be and driving out a pragmatic approach to mitigating risks.

Some examples of the key (but not exhaustive) areas to consider for significant risks in this area include

Security -- architecture can be completely undermined by a breach in confidentiality, integrity or availability of a solution. This area can be challenging to cost effectively mitigate so utilizing methods such as Threat Modelling can help prioritize security risks.

Capacity and Scalability -- effectively planning for customer and user demand can be challenging -- particularly for new or highly innovative solutions. Get the approach to risk on this wrong and you can lose customer trust.

Backwards compatibility -- managing the technology risk of users on older devices being shut out of the system

Data retention periods -- managing the regulatory risks of data privacy regulations such as GDPR

Need for high availability vs disaster recovery -- balancing the cost of the system vs the down time cost to the organization for the system being unavailable or rebuild in the result of a major incident.

It's worth considering that this process can be somewhat iterative. Mitigating some risks may lead to a change in stance on others. For example -- dealing with the risk of not having enough flexible / easily scalable capacity can be mitigated with automatically scaling cloud infrastructure -- which might then lead to revisiting legal risks associated with cloud. Options analysis and consideration of the risk trade offs is often required for the business to make an informed and balanced decision.

# Methods for Managing Risk

## Control Board and Risk Register / Log

Control boards are specified groups of accountable individuals who make collective decisions on risks. Control boards will often work through and review risk registers.

Risk Registers or Logs are effectively databases of risks that have been identified. At their most simplistic they can be a spreadsheet. All the way through to a full blown GRC (Governance, Risk and Compliance) platform that is specifically designed to manages enterprise risks.

## Controls and Controls Testing

Controls are specific techniques put in place to manage risks. Inspections, testing, validation, automated checks, backups, audits are all examples of controls that can be put in place. Controls testing and audits are undertaken to assess the effectiveness of controls. Architects may be consulted for advice on what effective controls could be put in place or what control testing could be used to verify the effectiveness of the controls. Whilst not exactly the same there is some similarity and overlap with QA and testing approaches and techniques.

## SWOT

SWOT analysis is a useful tool for identifying strengths, weaknesses, opportunities and threats, and thus can also help in identifying risks (with a particular focus on the Threat aspect of SWOT). The strengths and weaknesses refer to the internal factors, for example, a strong ability to deliver globally (strength) or long recruitment process (weakness). Opportunities and threats are external factors, for example, high demand for medical products (opportunity) or highly competitive market (threat). The organization has a greater degree of influence over the internal factors, and seeks to take advantage, or mitigate the external factors.

## Risk Matrix

Requires a re-write for the context of risk. "Assessing and managing risks is central to the feasibility and the success of a strategy. The level of risk may determine whether a strategy moves to execution or an alternative strategy is required. The early identification of risks enables mitigation, which can reduce probability and impact.

A risk matrix is a useful way to identify risks and rate them accordingly. Risks are listed in a column, and each risk is given a probability rating, from very unlikely (1) to most likely (5). A rating is also given for the consequences the risk will have if it is realized, from trivial (1) to critical (5)."

The values for probability and consequence are used together with the risk matrix to provide an overall rating, ranging from low to critical. After rating the risks, an assessment can be made of the strategy and tactics required to best provide mitigation.

# References and Further Reading

**Practical Risk Management Approach, PMI**
[Practical Risk Management Approach](https://www.pmi.org/learning/library/practical-risk-management-approach-8248){:target="_blank"}

**IRM's Risk management standard:**
[IRM](https://www.theirm.org/what-we-do/what-is-enterprise-risk-management/irms-risk-management-standard/){:target="_blank"}

**TOGAF Risk Management Chapter:**
[TOGAF](https://pubs.opengroup.org/architecture/togaf9-doc/m/chap27.html){:target="_blank"}

![image001](media/by-nc.png)

BTABoK 3.0 by [IASA](https://iasaglobal.org/) is licensed under a [Creative Commons Attribution-NonCommercial 4.0 International License](http://creativecommons.org/licenses/by-nc/4.0/). Based on a work at [https://btabok.iasaglobal.org/](https://btabok.iasaglobal.org/)