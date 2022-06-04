Architectural Analysis

Introduction

This section of the ITaBOK will examine the software architecture and infrastructure analysis. Architecture analysis is very important during the software architecture definition phase. The cost and the business implementation gets affected by the decisions which are made during this analysis.

Description

Software Architectural analysis is related to discovering important system properties using the system’s architectural models. It helps architects get clarifications from the customers regarding the key functional and non functional requirements. The architectural analysis helps the managers to ensure the project scope is within the budget and timelines. Architects can determine the component compose-ability by using the architectural models. The models helps the developers in knowing the implementation level decisions. The models help in locating and selecting appropriate components during the design phase.

The goals of the architectural analysis are ensuring completeness, consistency, compatibility and correctness in software architecture. Completeness is an external and an internal architectural goal. Completeness is external with respect to software system functionality. It is challenged by the complexity of the large scale system’s functionality. Completeness is challenged by different notations which are used to capture complex functionality. It is internal to architectural targets and modeling notation. Completeness ensures that all elements are fully modeled in the notation. It also ensures al the design decisions are captured.

Consistency is an internal property of the architectural model. It ensures that the model elements do not conflict with one another element. The different dimensions of the architectural consistency are name, interface, behavior, interaction and refinement. Compatibility is an external property of the architectural model. It ensures that the architectural model follows the guidelines and constraints of the style, reference architecture and a standard.

Correctness is another external property of the software architectural model. The model realizes a software specification. The implementation of the system realizes the architecture. System might include different structural elements, functionality and non functional properties.

Architectural analysis is related to analyzing the data exchanged in the system. The data structure, flow and properties are defined in the data design specification. The architectures can be at multiple abstraction levels. The architectures can be compared based on the factors such as processing, data definition, interaction of the components, configuration and non functional properties.

Different architectural concerns are analyzed. The concerns are related to structural, behavioral, interaction and non functional characteristics. The type of analysis can be static, dynamic and scenario driven. The scenario driven analysis can be static and dynamic. The automation which is achieved in the architecture can be manual, partially, semi, and fully automated. The different stakeholders in the architectural analysis are architects, developers, managers, customers and vendors.

Quality attributes are related to the measure of excellence in the software architecture. The attributes define the state of being defect free. They are the system properties which are separate from the software requirements. Implementation of the quality attributes makes it simple to differentiate a system from a good one to bad one. Attributes are related to the factors which affect system behavior and design. The other factors which can be the quality attributes are user experience and design.

Quality attributes can be static and dynamic. Static Quality Attributes are related to the structure of a software system. They are directly related to architecture, design, and the code. The quality attributes are not visible to the system user. The quality attributes such as modularity, testability, maintainability affect the development and maintenance cost.

Dynamic Quality Attributes reflect the software system behavior during the run time. The attributes are directly related to the software architecture, design, code, configuration, deployment environment, and platform. The attributes such as throughput, robustness, scalability are visible to the system user.

Quality Scenarios are related to ensure the prevention of the fault from becoming a failure. The quality scenarios are source, stimulus, environment, artifacts and response. Source is related to an internal or external entity. The entities can be people, hardware, software, or physical infrastructure. These entities generate the stimulus. When the entities come on the system, the condition of the system is referred as the stimulus. Environment is related to the the conditions where the stimulus makes an impact. The artifacts are related to the system or part of the system. The sample artifacts can be processors, communication channels, persistent storage and processes. Response is related to the arrival of stimulus. Responses can be detecting faults, recovering from fault and disabling the event source. The response measure is calibrating the occurred responses. The measuring helps in testing the requirements.

Perspective

The popular software architectural analysis methods are listed below:

Architecture TradeOff Analysis Method

Software Architecture Analysis Method

Quality Attribute Workshop

Attribute Driven Design

Cost Benefit Analysis Method

In practice

Architecture Tradeoff Analysis Method is related to evaluation of software architectures. The evaluation is performed relative to the software architecture quality attribute goals. The evaluations reveal the risks associated with the software architectural decisions. They potentially affect the achievement of the business goals. Architecture tradeoff analysis method checks how well the architecture satisfies the quality goals.It also checks how the quality goals interact with each other and trade off against each other.This is a leading method in the area of software architecture evaluation.

## Here’s how to do it.

This analysis method takes three to four days. The stakeholders involved in the analysis workshop are the trained evaluation team and architects. The skills and the knowledge required to conduct the workshop are software architectural skills and business knowledge related to the system.

## What are the pitfalls

ATAM requires different stake holders to have an active discussion. They need to meet and make consensus regarding the architectural decisions. It requires frequent and long meetings with stakeholders. Hence it is a heavyweight process. ATAM is difficult to be used in real life as the participation of the stakeholders need to be minimal for evaluation of the software architectural alternatives.

For increased maturity

Software architecture evaluation method like ATAM can play a role in the award and contract phases. It can help lower the risks associated with the defined software architecture. During the award phase, ATAM can be used to evaluate the approaches to system architecture. It can also assess the strengths and weaknesses of the architectural alternatives. SWOT analysis helps in finding the risks to the program. After contract award, software architecture analysis is used for contract management.

## References and citations

[ATAM: Method for Architecture evaluation](https://resources.sei.cmu.edu/library/asset-view.cfm?assetid=5177)

[Architecture TradeOff Analysis Method](http://wiki.c2.com/?ArchitectureTradeoffAnalysisMethod)

## Author(s)![](media/843ff7b88914b8b140df10001a5cda59.jpeg)

## Authors

Bhagvan Kommadi is the Founder of Quantica Computacao & has around 18 years’ experience in the industry, ranging from large scale enterprise development to helping incubate software product start-ups. He has done Masters in Industrial Systems Engineering at Georgia Institute of Technology (1997) and Bachelors in Aerospace Engineering from Indian Institute of Technology, Madras (1993). He is member of IFX forum,Oracle JCP and participant in Java Community Process.

Bhagvan Kommadi founded Quantica Computacao, the first quantum computing startup in India. Markets and Markets have positioned Quantica Computacao in ‘Emerging Companies’ section of Quantum Computing quadrants. Bhagvan has engineered and developed simulators and tools in the area of quantum technology using IBM Q, Microsoft Q\#, and Google QScript. Company's focus is on developing quantum cryptographic tools which will be able to provide quantum proof data security, which will help the banking institution to protect their transactions.

He is a hands on CTO who has been contributing to open source , blogs , latest technologies stack like go, python, Django, node.js & java, mysql, postgres, mongo and cassandra. He is an Individual member of Oracle JCP : https://jcp.org/en/participation/members/K. He is the technical reviewer for Packt publishing and reviewed - building-serverless-python-web-services- zappa : https://www.packtpub.com/application-development/building- serverless-python-web-services-zappa . He has written Packt Publishing - Hands-On Data Structures and Algorithms with Go. He is writing a book titled “Quantum Machine Learning in Python”. He has presented in PyCon before on topics such as Adaptive Learning etc.,

[bhagvanarch@gmail.com](mailto:bhagvanarch@gmail.com)
