---
title: "AI Architecture"
keywords: 
sidebar: mydoc_sidebar
toc: true
permalink: ai_ml.html
folder: engagement_model
summary: "AI architecture "
tags: 
  - topic_area
  - AI
---
************Santhosh Gottigere***********************************************
#Introduction
An Era of Technology Intelligence with Supersonic speed: We are in the era of technology proliferation at a breathneck speed with Artificial Intelligency (AI) unlike never before. Proliferation of AI is catalyzed by two forces demand and the resulting cost decreases, each of which drives the technology to become even better and cheaper. Massive leap in cloud computing chips specially designed for AI in terms of massive GPUs values and their uncanny quality to execute training models with exceptional levels of parallel processing abilities has fueled the possibility of 'Scaling' the AI as a viable technology today with ease which was a major stumbling block for AI and its application in the earlier times.

AI Proliferation is Technology's Apple Iphone moment that will shape our day to day lives, disrupt work and drive changes in human behaviors. You cannot beat it so as well you join now!!

#Difference between Artifical Intelligence (AI) and Machine Learning (ML)
> Artificial Intelligence (AI) refers to a broad range of computational systems that can think, reason, and interact like humans. AI is designed to mimic human intelligence by analyzing data and making decisions or predictions based on patterns and trends. (same as listed below... no changes)
> Machine Learning (ML) is a subset of AI that enables applications or computers or systems to learn from the data and get better over time to perform a specific task effectively.

Pros and Cons of AI and its Proliferation
**Pros:**
> **Increased Efficiency**: AI can automate repetitive tasks, freeing up time for more strategic work, and increase efficiency in industries such as customer service, accounting, and logistics.
> **Improved Decision-Making**: AI can analyze large datasets to identify trends and patterns that may not be visible to the naked eye, enabling better decision-making in areas such as healthcare, finance, and marketing.
> **Improved Standard of Living**:  AI can make everyday life more convenient and enjoyable,improving her health and standard of living by analyzing medical images, detecting anomalies, and alerting doctors to potential health issues earlier, allowing for more effective treatment and prevention of diseases.
**Cons**
> **Societal Disruption**: As much enjoyment and convenience AI can bring into our lives, it will be a disruptive force that will change our work, deliver customer experience and reshape cognitive thinking and behavior in the coming years.
> **Technology Arms Race**: AI Proliferation has heralded the rise of widespread techno-nationalism in which multiple countries will be locked in an ever escalating competition to gain decisive geopolitical advantage. And the race will be multi-polar in nature. It's no longer a self-fulfilling prophecy. It's here and happening now.
> **Containment**: Rapid evolution of AI and its proliferation due to its OpenSource in nature, can do potential harms, an unfolding maze of consequences that no one can fully predict or forestall. 



***********SKG*******************************************************************

#Overview 
Artificial Intelligence (AI) refers to a broad range of computational systems that can think, reason, and interact like humans. AI is designed to mimic human intelligence by analyzing data and making decisions or predictions based on patterns and trends.

Examples of AI include:

* General AI: A type of AI that uses machine learning algorithms to analyze and make decisions from vast amounts of data.
* Machine Learning: A subset of AI that enables computers to learn from data without being explicitly programmed.

Here are three reasons why AI is important:

• **Increased Efficiency**: AI can automate repetitive tasks, freeing up time for more strategic work, and increase efficiency in industries such as customer service, accounting, and logistics.

• **Improved Decision-Making**: AI can analyze large datasets to identify trends and patterns that may not be visible to the naked eye, enabling better decision-making in areas such as healthcare, finance, and marketing.

• **Enhanced Patient Care**: AI can improve patient outcomes by analyzing medical images, detecting anomalies, and alerting doctors to potential health issues earlier, allowing for more effective treatment and prevention of diseases.

***Note: These points highlight only a few examples of the many benefits AI brings to various industries and applications.


#AI Architectures

##Generative AI

###Agentic AI

####MCP (Model Context Protocol)

**Problem Statement**
Agentic AI allows for models to not only generate text for a client / end user, but to perform actions on their behalf with NLP as the input API. There are a variety of different actions that a client / end user may wish the agent to perform, and each action requires:

> The model can communicate with the third-party system to perform the action
> The model has sufficient authentication / authorization from the third-party system to act on behalf of the user

**Technical Solution**
MCP (Model Context Protocol) is an open source standard that was created by Perplexity in early 2025, and has gained industry-wide adoption, that allows for (A) authentication/authorization, (B) action discovery, and (C) action execution. Third-party services which wish to make their API functionality discoverable and actionable by an agent can implement the MCP Server to facilitate the communication to their internal systems.

**Implications**
Because agents are non-deterministic, some third-party services are hesitant adopt MCP without having full control over all possible ways that agents may interact with their systems. An API-first approach that has been so popular in the technical industry has led to a deterministic view of system functionality, so it is no surprise that the non-deterministic nature of API is met with some resistance.

The other major criticism of MCP is that the authentication and authorization is distributed to each disparate system the agent needs to communicate with, rather than a centralized authority such as Microsoft Entra. Most large organizations only have a single IDP that all auth_n/auth_z requests must route through. This approach is still compatible with MCP if it is only used within an organization's walled garden, but this approach does not scale to the reality of all of the third-party systems that a user wants the agent to interact with. No organization is going to prevent the user from authenticating with a third-party service to perform a third-party action, simply because the organization has a centralized IDP but the action the user wants to perform isn't inside of the organization. MCP's decentralized nature embraces the inherently decentralized nature of Agentic AI.