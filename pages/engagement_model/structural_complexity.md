---
title: "Structural Complexity"
keywords: 
sidebar: mydoc_sidebar
toc: true
permalink: structural_complexity.html
folder: engagement_model
summary: "One of the fundamental properties of a Complex system is something that we cannot easily know or cannot easily control."
tags: 
  - value_model
---

> "Fools ignore complexity. Pragmatists suffer it. Some can avoid it. Geniuses remove it."
**Alan Perlis**
 
# Complexity definition

Many ideas exist on the definition of complexity. We find 'Complex' is defined in Cynefin, a framework created by Dave Snowden based on his works. Complex can also be found within VUCA, used by the US war college and created by Warren Bennis and Burt Nanus.

One of the fundamental properties of a Complex system is something that we cannot easily know or cannot easily control. Complex can be considered the result of a system with many independent agents acting in such a way that we cannot easily predict the outcomes through pure observation & fact, we need to rely upon models and assumptions. Such as the weather, whilst we understand the individual components and make up of a weather systems, and we can predict behavior within certain tolerances, we are yet to find the tools to accurately model to guaranteed precision how the weather will behave at a single point in time and space.

Most, if not all of the systems we use in technology today are not Complex, however the environments they operate within, are.

An acceptable definition of Complexity is something we do not yet have the tools to know and to understand, therefore we cannot easily predict patterns and behaviors.

## Guidance on identifying Complexity

Technology systems are 'Complex adaptive' not 'Complex systems'. We have designed and built technology systems therefore we have the tools and understanding of how they work. Technology systems may be 'Complicated', but they are not 'Complex'.

A 'Complicated' system could sit within a 'Complex' environment which may impact the system in unknown ways, therefore we can strengthen our response to these external factors through adaptation and behaving in such a way to make it resilient.

We respond to impacts from Complex environments by building 'Complex adaptive systems'.

Recognising that a system sits in a Complex environment is key to building the right level of resilience into system design. We look to the Cynefin framework to help us do this. (see Cynefin, D Snowden). The Cynefin framework helps us to identify the environment we are working within, and provides guidance as to the best treatment strategies to adopt to solve for issues in that environment.

We can also look to VUCA (Bennis/Nanus 1987), an acronym that draws out the key areas to consider when dealing with unpredictability. VUCA defines 4 different types of challenge characteristics that required very distinct and different responses. Defining whether our system environment is Volatile, Uncertain, Complex or Ambiguous or a combination of can helps us produce more resilient systems design.

Antifragile (Taleb Nassim-Nicholas) also provides us with a view on how fragility causes systems to fail, this introduces concepts on how systems can adopt properties to make them anti-fragile.

## Importance of designing complex adaptive systems and why Architects should care?

System failures are often attributed to unintended and unknown consequences due to an unexpected event. Whilst we build systems to withstand known failures through robust and thorough functional testing, we cannot test for the unknowns because we do not know they exist.

Unknown consequences come from Complex domains that we cannot predict outcomes for, so we cannot measure the complexity of the environment, and we cannot measure how probable or frequent problems could arise. This leads to a question of how can we assure systems resilience, when we cannot know all the possible things that could go wrong?

Whilst we cannot measure Complexity, we can measure how our system respond to Complexity.

It is important that Architects understand the systems and process they design will operate in Complex environments. This means that they will be subject to unknowns, and that the primary cause of a failure will not be something they will have tested for pre-release. Failure will likely occur due to an unexpected stressor event in the Complex environment. How well you system 'behaves' under those circumstances is it's measure of the systems Complex response, and it's adaptiveness to complexity.

If we think of the components of an aircraft system, it is not tested against every possible or probably external event, it is tested against the worst of those events. Pressure, Weather systems, Gravity. We build in redundancy to a level we feel comfortable will exceed the actual possible event, therefore assuming it will survive the worse. However, whilst our aircraft system can handle the worse expected conditions, can it handle the worse unexpected conditions, a missile strike from an unknown terrorist group, an encounter with a UFO, the sudden immediate disablement of pilot and co-pilot to fly the plane.  These are unlikely scenarios in our design; therefore, resilience is not built in and when these events happen, things will fail.

The laws of entropy in the universe determine that everything decays over time, our job as Architects is to provide robust systems and solution that do not materially decay during their expected lifetime of use. We must apply resilience where possible, we must apply redundancy where possible within the boundaries of context we are within. This means we do not unnecessarily overengineer solutions where the cost outweighs the benefits, however we do design solutions that are sustainable and robust to the Complex environment.

## Dealing with Complexity -- Method

Some key principles can be applied to any design to enable it to respond to Complex environment stressors making it more resilient to failure. We can also apply principles to gain opportunities and competitive advances from external stressors.

One key theme to resilient design is to decouple components to the minimum level necessary to remove cascade effects of a component failure. Many independent agents acting towards a common goal provides greater resilience than a large interdependent coupled entity. Think of a flock of birds migrating south for the winter to survive, if one bird fails to make the journey, the flock still arrives south and can continue to thrive.

**Assessing Complexity**

Use Cynefin & VUCA to assess the environment the systems sits within. Use VUCA/Cynefin treatments strategies as a base for your design thinking.

**Software systems complexity**

Applying techniques of Antifragile Software systems (K. Hole) and understanding residual theory (Barry O-Reilly) can help us design software systems to become more resilient to external Complex environments. Some key focus areas to consider:-

Decoupling independent agents, reduce dependencies between agents to reduce the 'chain effects' of a negative event.

Applying diversification to codebase -- develop multiple routes to achieve the same event, build in appropriate monitoring to identify failures and re-route procedures through other pathways if the primary fails.

Apply queuing techniques to data manipulations, using publish subscribe will conserve independency of agents, using event-based architecture techniques will also support to preserve individual components.

Choreography design -- design components that can work alone to deliver a task, but can integrate into the wider software ecosystem working collaborative with other components to deliver a wider objective, yet remaining independent of other components.

Use Service Orientation Architecture techniques to decouple major services is good practice.

Do not apply reuse where possible. Novelty has proven much more successful when dealing with Complexity. Just because a particular solution addressed a known problem, does not mean it will address a similar problem in a Complex environment.

Understand the external stressors on the software base from a Complex environment perspective building mitigation where necessary. i.e. what happens to our core accounting system if there is a pandemic and people cannot attend on site to maintain the system?

**Testing your architecture**

Testing the design or architecture of a solution, prior to build, is an essential step. Ensuring you have adopted the key principles of decoupling, diversification, stressors, consider: --

Applying a *Design Structure Matrix* to each component in your architecture to test which components have high dependencies and cannot operate independently, treat accordingly with further decoupling or revisit design.

Apply FMEA: (*Chris Cooper Bland to add)*

Undertake desk-based stress testing. Find out what are the key stressors that could affect your design, as well as interviews with stakeholders, think of non-obvious stressors that could impact the system, Pandemic, earthquakes, regulation change, loss of key resource.

Stressors are NOT [risks](risk_methods.md){:target="_blank"} and we do not measure the probability of the stressor happening, we assume it will happen and ask "How would the system behave under the conditions of this stressor" -- adjust design accordingly.

Apply context to your [design](design.md){:target="_blank"}. Think about how impactful particular stressor could be should they occur. For example, a global communications system would be very important in a disaster scenario such as a meteor impact, however this stressor would be less impactful to the ordering system for a local Pizza shop.

## Summary

Architects should have a basic understanding of Complexity and how it impacts design.  It is important to differentiate Complexity (unknown, unpredictable), from Complicated (known, just very difficult).

Complex environments need trial and error to solution for, novelty is important here as we try new things to create desirable outcomes, creativity is important as a lack of proven trusted process is available and reuse not always applicable to address the problem.

Dealing with complexity requires adaptability, agility and innovation. Be prepared to continuously adapt designs and be wrong. Constantly ask questions "What will break this design?", "What are the impacts?", "Does it matter?".

# References

**Dave Snowden -- Cynefin**

**K Hole -- Antifragile in software systems**

**Taleb Nassim Nicholas -- Antifragile**

**Barry O' Reilly -- Residual Theory**

**Browning, Tyson R. (2016) "Design Structure Matrix Extensions and Innovations: A Survey and New Opportunities,"**

**Igor Nikolic Intractability**

![image001](media/by-nc.png)

BTABoK 3.0 by [IASA](https://iasaglobal.org/) is licensed under a [Creative Commons Attribution-NonCommercial 4.0 International License](http://creativecommons.org/licenses/by-nc/4.0/). Based on a work at [https://btabok.iasaglobal.org/](https://btabok.iasaglobal.org/)