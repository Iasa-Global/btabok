---
title: "Dissecting Design"
keywords: 
sidebar: mydoc_sidebar
toc: true
permalink: design_overview_1.html
folder: btabok_overview
summary: "Tools for adopting the btabok in everyday practice."
tags: 
  - digital_business
  - engagement_model
  - 
---

# Dissecting Design - Introduction

So this was my first time using an AI generated image for a blog... have to admit I'm not super impressed. The first one it generated was somewhat spooky and distopian... off of the this text: "design tools and computers and diagrams creative work people who do the work cartoon lines diagram happy people process and technology"

![No alt text provided for this image](https://media.licdn.com/dms/image/D4D12AQFDrfal86c_Zw/article-inline_image-shrink_1500_2232/0/1670866960560?e=1685577600&v=beta&t=EIMck57vFMdyzHCS9G6BMf7TSyocYDFiW7XtrrSqYPo)

This is a bit nightmarish

Will keep playing with it. On to the article.

Design methodologies for architecture are relatively difficult to find, especially those that relate to both technical and business outcomes. One of the goals of the BTABoK was to create a ‘method to the madness’ for current architects and architecturally significant decisions. Keep in mind, in this article, we are referring to the design of the combination of business and technology areas, so the design of a purely manual business process is not part of our consideration (see Iasa’s definition of architecture). We are going to discuss the following model for design relationships and a structured approach using the BTABoK structured canvas approach.

![No alt text provided for this image](https://media.licdn.com/dms/image/D4D12AQEYjCZXpjMwVg/article-inline_image-shrink_1500_2232/0/1670866361653?e=1685577600&v=beta&t=cVdslYIc6PTCg_vKZ4J2fQRxM4n0eEdEgiJdG7_JGtc)

Taken from BTABoK Design Article: https://iasa-global.github.io/btabok/design.html

So what is this diagram? In the context of architecture, we often talk about design as a single thing. We design software, we design automated build environments and web design services. However, the design turns out to be a complex set of interactions with design decisions, requirements, and options for a decision. These are further complicated in their relationships to the overall solution space. The larger the [Scope](https://iasa-global.github.io/btabok/scope_context.html) of the solution space, the more complex the set of relationships.

As we consider a design, the most important outcome of this process is not the models we use but the decisions we make. These decisions are what lead to value outcomes like business benefits, risk, technical debt, etc. These decisions flow through the delivery process and ultimately control the maximum amount of value derived by our client for the solution. (Article on Clients?). These decisions are at the core of what great architecture is all about and why architects study more than just technology or cost factors in design.

Keep in mind that a) not all decisions in a solution space are architecturally relevant, b) decision input is often facilitated across teams or experts in a depth areas, and c) most decisions link to other decisions and must be balanced (conformance) across the solution. One great architect I met said our job is to make sure that ‘no one gets everything they want, but everyone gets enough,’ which I hit very close to home.

## Requirements

So we talk about stories, epics, requirements, use cases, and all of the other names used to describe a thing we want the solution to look like, taste, link, withstand, function like, etc. The BTABoK uses Architecturally Significant Requirement because it is the most recognized in any methodology (though we have specific cards matching with Agile Architecture). I think it is easy enough to show what an ASR looks like for you to understand what makes it significant.

![No alt text provided for this image](https://media.licdn.com/dms/image/D4D12AQHrF9y5gLbfCQ/article-inline_image-shrink_1500_2232/0/1670866339902?e=1685577600&v=beta&t=48-ivWo6AqXxDQdNG1_E7jb7rMC2cH-lDXbAfcuBOPU)

ASR Card from Requirements (https://iasa-global.github.io/btabok/requirements.html)

As you can see, what makes an ASR ‘architectural’ are its characteristics. Cost, novelty, risk, etc. In addition, ASRs come in multiple types. Functional ASRs provide clear functionality which can be linked directly to a business objective (OKR). Quality Attribute ASRs are those that provide cross-cutting impact on structural outcomes like performance and reliability. Finally, constraint ASRs may link to an architectural principle, a standard that must be followed, or other constraints which limit the options open for the design decision. For example, if the solution must be PCI compliant.

Design is partly the act of deciding on a solution to an ASR. However, ASRs are not in themselves valuable unless they can be measured. So it is essential in design that the requirement be linked to an OKR or a fitness function which can be measured against risk or impact to the solution functional requirements such as performance.

## Options

Anyone who has designed systems (or even dog houses) knows that once you start reading or making requirements, a bunch of options pop up in your head (‘we could use React, hmmm or React Native, Angular, Vue, or others?’). These options just can’t help but pop up even in the most basic description of a solution design space. 

Options come in many forms. Technology breadth includes the options of using different technologies in the solution design space. Technology depth relies on deeply understanding a technology choice and being able to utilize it for maximum benefit and the strongest quality attribute support. Patterns are reliable solutions to common implementation problems. Reference models are a grouped set of design decisions and patterns within a technology space, normally within a technology depth area. (the next article will cover Design Options in depth).

![No alt text provided for this image](https://media.licdn.com/dms/image/D4D12AQE17dzEtIq69Q/article-inline_image-shrink_1500_2232/0/1670866313882?e=1685577600&v=beta&t=HpfmticHW1p5Gz7ZaidGyCdV2PXQdWbh-SUr6FzMGNM)

Design Landscape Canvas

The design landscape is a set of three canvases that lay out WW02 or TOGAF technology stack. But instead, it lists all the types of technologies that you might want to implement based on a requirement, but in their generic ‘technology type’ kind of way. The goal of the design landscape is to help think about solutions without thinking about products or specific technologies. This helps to set up the solution to the requirement without getting bogged down. Think of it like a flavor wheel in a wine tasting… it helps you think about things you *might* need and then asks you to *decide* if you really need it. As you will see in a future article, if you were doing this process sequentially as opposed to the web-worked fractal that is creative thinking, you would use these icons to populate a context view of the solution. But let’s save that for part 2 or 3.

## Decisions

Decisions are the heart of architecture. If requirements help us shape the objectives, then decisions help us sculpt the final graceful curves of the finished product. All too often, models are considered architecture. Here is a reference model from MS Azure…

![No alt text provided for this image](https://media.licdn.com/dms/image/D4D12AQHcraHH4dDzHw/article-inline_image-shrink_1500_2232/0/1670866192843?e=1685577600&v=beta&t=-ngGDSu7aioAtuNXgoQR581Tl9CkjISzy9N_nBJnUrw)

Azure Reference Architecture

If you were shown this diagram, you might be told, ‘this is an architecture for a Highly Available Web Application. However, those of you familiar with modern architectures in Azure would immediately spot the problem with the diagram… Namely, that it is OLD. It has been updated since to recommend what Microsoft considers to be today’s decisions. The current model looks like this:

![No alt text provided for this image](https://media.licdn.com/dms/image/D4D12AQFbQd-xphreew/article-inline_image-shrink_1500_2232/0/1670866207719?e=1685577600&v=beta&t=Lbb9sCEXs8NzVwd5Noe3VLl2OmrSUQgyHInbVoT4X0Y)

Up-to-Date Reference Architecture

Any programmer will tell you this is a *MUCH* different beast. We have added service buses and changed the API App and Web Job into a Service Bus and Function Application. So what’s the big deal? *WE HAVE NO IDEA WHY!* This change in decisions will make the application functionally different, it will work with different cost profiles and state management, will require the use of a drastically different way of coding, and will likely lock us into Azure (hmmm, now why would they do that? 😊). I could duplicate this example a dozen times from a dozen different vendors, solution design, and real-world projects.

Decisions, not models, are the snapshot of architecture, though, of course, we still love models which help us understand and get to the decisions. Enter the architecturally significant decision record. The ASD as we fondly call it, is a workable one-page decision management engine. In future installations of this series, we will show the scope and numbers of ASDs (and ADRs) on different products with different complexity estimates.

![No alt text provided for this image](https://media.licdn.com/dms/image/D4D12AQGqjlyc-O8E8w/article-inline_image-shrink_1500_2232/0/1670866229653?e=1685577600&v=beta&t=u1_ZDgJDD-wcKPtzoF77-54KK9y_XTIsHcVSl2QfPWY)

Architecture Decision Record Template

The ADR is a bit complex, and we will have a couple of articles dedicated to it (as well as the spin-off versions in excel and markdown), but for the time being, notice the big sections. The top area describes the decision and links it to a requirement this ensures that we are working through traceability and not just design overload. It also describes the scope of the judgment, which will impact the next area. The right column defines HOW the decision will be made. How reversible it is, how long we have to make the decision itself, what information quality we need (never 100%!), and the effort we will put into it. In addition, we can describe the owner, the process, the authority type, and the consequences. This thinking helps us shape the decision from a 1 hr whiteboarding (or canvas and sticky notes) to a year-long study.

The card obviously has three options (why three and not 2 or 4? Limited space and time) and the areas on which we will compare them. Areas are the things like cost, support, existing skillset, etc., that will allow us to show WHY we made the decision. Here is a mocked-up example of the previous serverless decision:

![No alt text provided for this image](https://media.licdn.com/dms/image/D4D12AQFuvY21DQ-aEQ/article-inline_image-shrink_1500_2232/0/1670866257351?e=1685577600&v=beta&t=B6uU0uAPR8A31szhEX8TYrhSExwxgy33NtaZXAHdE1k)

Mock Example of an ADR

You can find all of these canvases in a mocked-up miro board of the Iasa canvases we will be covering in these articles here: [Miro | Online Whiteboard for Visual Collaboration](https://miro.com/app/board/uXjVORNRx4s=/?share_link_id=155880042988).

I am looking forward to this Design Series based on the BTABoK. Here is my current thinking on the order they will come in:

1.     Dissecting Design – And Introduction

2.     Options, Options, Options – So Many Choices

3.     Deceptive Decision Making – Why Agile Architecture is so Hard

4.     Views and *BEYOND* – Thinking, Facilitating, and Communicating

5.     I Like Patterns – Patterns, Reference Models, and Conformance

6.     Assessments, Tests, and Chasing Perfection – How Governance and Architecture are Different
