---
title: "Principles"
keywords: 
sidebar: mydoc_sidebar
toc: true
permalink: principles.html
folder: engagement_model
summary: "Principles can be seen as the experiential rules we have learned as an organization to guide *how* we construct efficient solutions or how we try to frame decisions we come across repeatedly."
tags: 
  - value_model
---

> "A basic idea or rule that explains or controls how something happens or works"
**Definition of Principle, Cambridge Dictionary**

# Architecture Principles Overview

There are a huge number of decisions that need to be made in any project, and a good set of architecture principles can make dealing with these a lot simpler by providing context and direction in important areas. An appropriate set of architecture principles also supports agile product development in a way that a prescriptive EA target architecture does not, as they draw boundaries but let the teams produce creative designs with that space. 

Principles can be seen as the experiential rules we have learned as an organization to guide *how* we construct efficient solutions or how we try to frame decisions we come across repeatedly.  They represent how the organization delivers the highest value to customers and what those customers see in our technology choices that enable them.  Many technology focused organizations need multiple sets of principles as they grow, and over time:  for instance, a small IT department might need only one set of rules whereas a larger technology product organization might need overall enterprise/product architecture standards as well as solution architecture principles and specific sets for security, data and such. In organizations which provide very diverse products or services there may be differing sets per domain, dependent on business context or [Quality Attributes](quality_attributes.md){:target="_blank"}.

IASA recommends starting with a small set (8-12) of written statements to guide the important decisions that need to be made in many projects and as the value of principles are seen in different areas grow this over time.

# In practice

In this section, we'll describe what a good principle looks like and show how to get started with a blank "canvas" and start writing up our principles.

Principles are expressed in simple language, usually in one or two sentences. A good principle is:

-   constructive (it helps to drive decisions forward and highlight issues)
-   compelling (it is strongly motivated by drivers, goals and other principles)
-   memorable (it is clear, concise and understood)
-   testable (we can determine if it is being followed)
-   decisive (it unambiguously sets direction)
-   useful (it is not a truism: could the opposite ever be true?)

The key to developing a useful set of principles is gaining *buy in* by collaboration, this is a team activity.

Principles should link the business goals to the decisions made on the programme or project

The diagram illustrates in particular one of the key benefits of developing principles: they can be used to justify architectural decisions right back to business goals.

Architecture principles are there to help projects arrive at the best solution for the organisation, however they may not be applicable is all cases. If there is a principle which seems wrong for your project, challenge it, don't just follow blindly and do the wrong thing.

A fully formed principle is comprised of:

-   An easy to remember title
-   A statement describing what the catchy title means
-   Rationales to justify or explain the motivation for the principle, that is, why it has been adopted. Many rationales themselves are business drivers or other principles
-   Implications or the consequences or outcomes of adopting the principle. Many implications turn into further principles themselves.
-   Actions which the principle drives
-   Exceptions, if allowed for tactical reasons, are specified
-   Source of the principle

As we said, the number of principles in a principles set should not be large, 8 to 12 is a good number. If an organisation has more than this, they might be being too prescriptive or the principles need to be broken down into subsets, for example, there are EA principles, data principles, security principles, etc., which are useful for different stages or areas of the design.

## Here's how to do it. 

No particular knowledge is required beyond a basic understanding of the organization's culture and knowledge management practices.  Constructing a principles set is a multi-stage process, a good place to start to capture the statement of principles is a simple list.  The first stage is to identify the [stakeholders](stakeholders.md){:target="_blank"} who should be involved (Link to Stakeholder doc), these will typically be the technical decision maker and their advisors.

The architect should call a meeting and have the group discuss the following sections, often in order first, and then with general discussion to revisit problematic areas:

Create a list

1.  Canvas the team for examples of architectural principles
2.  Identify key business drivers (relevant to the group) -- can be key words or phrases like "Grow market share" or "Focus on quality products"
3.  Establish the goal for creating a list of principles (possibly reviewing some examples)
4.  Brainstorm key principle titles -- can be single words or phrases like "knowledge sharing," "opt for lowest cost," "in compliance wherever we operate," or "predictable."
5.  Split into smaller groups or individuals to write a short description for each -- no longer than 50 words.
6.  Review the complete list and ask external organization members to suggest any gaps or unclear areas.

Complete the canvas for each principle

-   The smaller groups complete the canvas for each principle
-   Review the completed canvases and ask external organization members to suggest any gaps or unclear areas.
-   Team reassembles to complete the version and convert to a shareable graphic/web site/etc. for sharing with the broader organization.
-   Update the architectural governance process to include the use of principles and ensure they are updated.

This process should take a 2-6 meetings, some basic supplies (post-it notes, flip charts), some graphic communication technique familiarity (communications).

## What are the pitfalls

There are several potential areas where creating a set of effective principles can fail:

1.  Other leaders do not buy-in to the principles and are not willing to practice them
2.  The architects and engineering teams involved do not know how to implement the principles and cannot make them part of their personal practice
3.  The socialization of principles or ethics becomes a paralyzed process and potentially leads to arguments
4.  Architects or designers will blindly follow a principles which is plainly wrong in this context.
5.  Too many principles could show that either the requirements are not clear or that principles are too narrow in scope (too specific, becoming rules), thus creating a rigid context → more generic principles should be defined instead
6.  Too few principles would make harder to trace the decisions back to requirements and also blurs the [scope](scope_context.md){:target="_blank"} of architecture

These problems are all about collaboration and understanding, which is why the workshop approach is important. Then there needs to be socialization and education, discussions with case studies or examples may be helpful. To avoid this taking too long set a timeline for the first version to be drafted, making sure the goal is understood by all participants, and meeting facilitation techniques are employed. Having a published revision process will help with acceptance, as we can refine the principles later as well as making sure they stay aligned with business and technology strategy.

Do note that the Dilbert cartoon strip and others which have their roots in modern corporate behavior often show antipatterns in principles -- which are both human and altogether common.  These can be a useful way to start discussion without being perceived as either boring or negative.

# Examples  

Principles do not generally depend on other areas of the BTABoK and instead often inform those areas.  In this section, we describe some sets of architecture principles.

## Enterprise architecture principles

The EA perspective often blends the ethical obligation to external customers and stakeholders with internal business principles (how the organization comes up with solutions in a technical sense).  The following set of principles was adapted from a council of global manufacturers to describe how solutions would be preferred:

| Sample principles list for the business to technology transition:   |

In general, the understanding of these would guide architects towards selecting solutions which met #1 (safety [to human life], disaster resilience, and compliance) first.  Then the second criteria would be evaluated, and so forth.  If a solution or program did not meet the first three criteria (without exception), it would be rejected.  This systems-level view added to a corporate culture (which had a strong ethical similarity between the manufacturers -- a commitment to the customer), and provides a more day-to-day interpretation of *how a group might align decisions*.  This also helped the architecture teams expose this thinking to the business units in order to be more predictable over multiple initiatives.

## Solution Architecture Principles

The second example here is a set of principles from a high-tech manufacturer's global IT team used to orient new technical or business architects.  I would like to thank Jared Kunz for his original work here and discussions in refining this.

| Sample principles list for the business or technical architect:   Understand and follow these (in no particular order): [The ISC^2^/CISSP Code of Ethics](https://www.isc2.org/Ethics){:target="_blank"} (abbreviated items, my favorites)Protect society, the common good, necessary public trust and confidence, and the infrastructure.Act honorably, honestly, justly, responsibly, and legally.Provide diligent and competent service to principals.   [The 10 Commandments of Computer Ethics](https://en.wikipedia.org/wiki/Ten_Commandments_of_Computer_Ethics){:target="_blank"} (abbreviated items, my favorites) Thou shalt not use a computer to harm other people. Thou shalt not interfere with other people's computer work. Thou shalt not snoop around in other people's computer files. Thou shalt not use a computer to steal. Thou shalt not use a computer to bear false witness.Thou shalt always use a computer in ways that ensure consideration and respect for other humans. Strive to be a genuine servant leaderIf you make a mistake, own up to it, where applicable, apologize, do your best not to repeat, if you repeat, seek help, remove yourself from the recurring situations.Smile, laugh as appropriate, stay positive and have fun (within the bounds of ethics and laws).Be curious, experiment -- try new solutions but reduce the time required to validate the results.Bring the best facts and the best data for the situation and your audience, know your audience.  The facts and data speak volumes and often at much higher decibels.Business Terms, Business Facts, Business Rules, can't run a business without them, yet many leaders of business don't even know they existA healthy business recognizes and values its information resources (data, applications, technology as well as people) and these resources are valued and managed like any other critical business resources.The fundamental problem with "systems thinking" or looking at the world from a "systems" or "application" or "object" view is that processes and data are orthogonal.  Processes, data are very free flowing, they cross many boundaries of systems, boundaries of what people want to draw lines around into "applications" so there are many better ways to manage processes and data than just "systems" and "applications".  Microservices, event driven, cloud, and continuous integration architectures are an answer to the limited way of "systems" thinking due to the complexity of processes and data flowing freely.Aim to provide detailed designs to a majority of stakeholders at the last responsible moment: When applicable, leverage the advantage gained by reasonably delaying some architectural decisionsRationale -- Additional information may become available, priorities may change. Avoid thinking you can predict the future and over-engineering the design. Reduce or completely eliminate through your designs the amount of [technical debt](technical_debt.md){:target="_blank"} Find the appropriate level of data, process and software couplingStrive to design self-healing systems that can monitor/repair themselves Design to limit propagation of failures with proper monitoring, alerting when failure propagation limits are difficult to design.   |

This list is more easily composed by a lead architect for his team or for his immediate customers.  In lieu of organization-wide principles, the architect can still define some of his or her immediate environment and show themselves as technical leaders through example.

| Move Data to the Edge Statement -- It is important that data resides as close as possible to where the client needs it, whilst maintaining integrity and availability. In a global solution this results in highly distributed systems. Rationale The key reason for this is to give fast response times which don't depend on how far you are away from the data centre. It also supports high availability requires of the organization by limiting the impact of any regional failure. Implications Systems will be distributed which results in more complexity.Technologies such as CDN will be essential We need to understand what data is needed where and what the data governance requirements are, for example if data must be encrypted or must be held in specific geographies Actions Identify the recommended CDN for the organization.Define data distribution strategy Exception Until the CDN is identified the System of Record will remain with the existing system. Source Workshop in XX on XX   |

Fully Furnished Principle:

# Classification of Principles

Principles define direction within a certain scope, in some cases this can be part of an inheritance model.  For example

Enterprise level Principle:

**IT is an enabler**
Statement: In the fast changing business context in which the company operates, where first-mover advantage is key, IT must support the business with a rapid path to production

Solution Architecture Principle:

**[Agility](agility.md){:target="_blank"} is key**

Statement: An agile delivery method must be adopted, automate everything, use CI/CD

Application Architecture Principles:

**Use containers**

**Deploy on cloud environment**

## Categories/Subsets

For a better understanding, architecture principles can be also organised in subsets (or categories): *Business*, *Application*, *Information*, *Technology* (see [TOGAF](http://pubs.opengroup.org/architecture/togaf9-doc/arch/chap23.html#tag_23_06){:target="_blank"} and an example from [University of Birmingham](https://intranet.birmingham.ac.uk/it/documents/public/architecture/Enterprise-Architecture-Principles.pdf){:target="_blank"}

Since** the goal of architecture principles is to support the business objectives (concerns) within the given constraints**, there are cases when adopting one principle will filter out other principles -- since they will either conflict with each other or exceed the limits of a constraint.

For example, a specific architectural style (layered architecture, micro-services etc) is normally an architectural decision and, as such, it represents the output of applying one of the architecture principles. However, there are situations when the architectural style is given as a constraint (i.e. requirement) -- instead of emerging as a decision following an analysis exercise. In that particular case, some of the existing architecture principles cannot be adopted since they will conflict with the given style -- which acts as a constraint and filters out other principles.

As it was mentioned, architecture principles are used to trace the architectural decisions back to the business goals (i.e. requirements). Since business goals are different across various business domains, having different constraints (regulations etc.), it is possible to create specific architecture principles sets for business domains: Financial, Health, Retail etc. (an example on [ibm.com/developerworks/](https://www.ibm.com/developerworks/rational/library/enterprise-architecture-financial-sector/index.html){:target="_blank"} for Financial sector)

# Perspective

There are a number of organizations -- both in the public good and commercial -- who have advanced statements of principles, listed below.  In this section, I am going to summarize an elevator pitch I heard consistently while at Boeing.  I asked the group of architects I was talking with how they prioritized principles and they almost unanimously replied with this simple statement, "We do:

First, what is right for our customer [to be safe, see value in our solutions, ...]

Then, we do what is right for Boeing as a company,

Finally, we look at what is right for our own work group."

Ask around your organization and see what answers you might get.  One of my own teams (which had had some ethical issues pin the past) came back with a completely reversed order and I realized that we had a significant gap in our shared understanding of these core principles and how as a group we understood them. 

If an organization's principles illustrate how they decide, what are your principles?

# References and citations

**Please take a look at the following examples and sources:**

**University of Washington**
[https://www.washington.edu/uwit/divisions/isss/ea/ea-guiding-principles/](https://www.washington.edu/uwit/divisions/isss/ea/ea-guiding-principles/){:target="_blank"}

**TOGAF**
[http://pubs.opengroup.org/architecture/togaf8-doc/arch/chap29.html](http://pubs.opengroup.org/architecture/togaf8-doc/arch/chap29.html){:target="_blank"}

**Agile architect**
[http://www.agilearchitect.org/agile/principles.htm](http://www.agilearchitect.org/agile/principles.htm){:target="_blank"}


**Matt Kern and agile principles**
[https://www.linkedin.com/pulse/post-agile-principles-matthew-kern/](https://www.linkedin.com/pulse/post-agile-principles-matthew-kern/){:target="_blank"}


**AWS hiring principles**
[https://www.amazon.jobs/en/principles](https://www.amazon.jobs/en/principles){:target="_blank"}

![image001](media/by-nc.png)

BTABoK 3.0 by [IASA](https://iasaglobal.org/) is licensed under a [Creative Commons Attribution-NonCommercial 4.0 International License](http://creativecommons.org/licenses/by-nc/4.0/). Based on a work at [https://btabok.iasaglobal.org/](https://btabok.iasaglobal.org/)