---
title: "Analysis"
keywords: 
sidebar: mydoc_sidebar
toc: true
permalink: analysis.html
folder: engagement_model
summary: "Analysis of the architecture helps us to understand the nature of that compromise.  Many of the architecturally significant requirements are expressions of desired quality attributes."
tags: 
  - value_model
---

> "Analysis is the art of creation through destruction."
**P.S. Baber, Cassie Draws the Universe**

If the purpose of an architecture is to "provide a framework in which to satisfy the requirements and serve as a basis for the design", then it follows that we need to be able to analyze candidate architectures to determine how well they carry out that purpose.  IEEE recommends using architecture descriptions "as basis for review, analysis, and evaluation of the system across its life cycle" and "as basis to analyze and evaluate alternative architectures".  This article explores the reasons for analyzing an architecture and possible alternatives and describes how we go about it.

An architecture can be seen as a representation of a set of architecturally significant decisions that come together to address a significant business requirement.  These decisions are not independent of each other, and the sum of them, describing a system or service as a whole, is greater than the sum of its parts.  So one cannot simply decompose the problem, address each architectural requirement individually, and hope that the resulting architecture is coherent.  The ways in which requirements and solutions are interconnected are brilliantly described in Christopher Alexander's *A Pattern Language,* where 253 design patterns form a web connecting all the way from the selection of items to hang on the walls of your living room to the distribution of towns across a region.  IT architecture, in this respect, is no different.

Unfortunately, in most situations, the requirements that together make up the overall business requirement are, to a greater or lesser extent, in conflict with each other.  To take a very simple example, the desire for a system to be easy to use might conflict with the desire to make it secure.  There is no "correct" resolution of this conflict, as it depends on the context.  One might choose one trade-off between the two for a banking application but adopt a different solution for a simple information service that does not involve personal data.  Many such conflicts might exist among the requirements of a system or service, and a preferred architecture can be seen as a solution that delivers value, but is nonetheless an inevitable compromise.

Analysis of the architecture helps us to understand the nature of that compromise.  Many of the architecturally significant requirements are expressions of desired quality attributes.  Can we live with the limitations that the compromise represents?  By how much will the value of the solution be reduced as a consequence of achieving reduced levels of some desirable quality attributes?  Might there be ways of mitigating these deficiencies?  Or might an alternative architecture, representing a different set of compromises, deliver greater value overall?

**Trading-off quality attributes**

In 1995, the Software Engineering Institute at Carnegie Mellon University (SEI) suggested the use of quality attributes to facilitate the analysis of alternative software architectures.  The Software Architecture Analysis Method (SAAM) was "the first documented, widely promulgated architecture analysis method".  It was originally created to analyze an architecture for modifiability, and requires the creation of a set of scenarios that illustrate what sorts of modifications to a software system are likely or representative of a given domain.  Candidate architectures are then evaluated according to how well they support the set of likely modifications or benchmark tasks.  A number of similar methods followed, and in 2000 the SEI extended SAAM to consider multiple quality attributes with the Architecture Trade-off Analysis Method (ATAM).  ATAM has become quite widely used by software engineers and architects to evaluate software intensive architectures.  The use of quality attributes allows an evaluation team to "see the wood for the trees", preferable to trying to examine a large number of individual requirements, while the expression of quality attributes, which can seem somewhat abstract, in the form of scenarios ensures that they are concretized and placed in the context of the system under consideration.

**Involving the stakeholders**

Powerful stakeholders can influence architecturally significant decisions, and many stakeholders will be affected by the outcome.  So it makes sense to involve stakeholders in the analysis process, both as contributors to the requirements and to the evaluation of alternatives so that they can understand the compromises and trade-offs involved in selecting a preferred architecture.  A successful analysis is therefore unlikely to be an exclusive affair involving only architects, and to be inclusive it must involve a language that all stakeholders can become conversant with.

**Finding a common language**

Wikipedia lists over eighty differently named system quality attributes, some of which would struggle to find a place in an English dictionary, and many of which overlap in their meanings.  This diversity of language is perhaps evidence that professional practices among IT architects are emergent and have not yet reached the stability that might be expected in a more mature professional community.  It is possible to significantly narrow down this language, making it more accessible, while still ensuring a coverage of all aspects of system quality with a minimum of overlap.  ISO 9126 contained just six quality attributes, broken down further into twenty-seven sub-characteristics.  In 2011 it was superseded by ISO 25010 which expanded a little to eight quality attributes and thirty-one sub-characteristics.  Adoption of a common language by an organization helps achieve consistency between different analyses, making it easier for stakeholders to become increasingly fluent in the language, and creating the possibility of comparison between analyses.

Another element of the required "common analysis language" is the expression of how well or badly a given architecture satisfies a requirement or quality attribute.  Most methods, including ATAM, adopt the economic concept of *Utility*, generating utility trees to guide the exploration of risks, sensitivity points and trade-offs across alternative architectures.  The notion of utility can seem rather abstract, and an alternative approach, that borrows from a language well understood by business leaders, is to express the degree of satisfaction in terms of risk.  Many corporations manage and quantify risks using the formula *risk exposure = risk impact x risk likelihood*, an approach, developed by Dutch mathematician David van Dantzig, that was adopted to assess flood risk in 1953*.*  The Solution Architecture Review Method (SARM) presents an evaluation of alternative architectures in terms of risk trade-offs between quality attributes and their underlying architecturally significant requirements.

**Putting it all together**

We've covered the basic ingredients for an architecture analysis: identifying the stakeholders, understanding the architecturally significant requirements (ASRs), relating these to a quality model that describes the desired quality attributes and defining a language that can be used to describe how well or badly a given architecture satisfies the set of requirements.  The assembly of these ingredients into a process is simple, though it does place significant demands on resources.  If it seems rather expensive, spend a moment or two to consider the ultimate cost of making the wrong architecturally significant decisions.

A typical architecture analysis process involves the following steps:

1.  Identify the relevant stakeholders.  It is a good idea to understand the different types of stakeholder involved, using one or more of the stakeholder analysis techniques described [here](stakeholders.md){:target="_blank"}
2.  Document and classify the relevant quality attributes and architecturally significant requirements.  This is often done in a workshop bringing together stakeholders who can gain a useful appreciation of each other's different perspectives on the system or service.  You can find more guidance on ASRs [here](requirements.md){:target="_blank"}.  This creates the context in which the analysis will take place.
3.  Understand the architecture or architectures you want to analyze.  Architecture  can be used to explore an existing architecture to better understand how well it meets its needs, or to consider alternatives.  It can also be used as part of a procurement process, injecting architectural thinking into the evaluation that might otherwise only focus on functionality.  The ASRs captured in the previous step can inform the formal Request for Proposal (RFP), while the evaluation workshop in the next step can become the technical evaluation of the RFP responses.
4.  Conduct a trade-off analysis.  This involves understanding how each candidate architecture will perform against the desired quality attributes and their associated ASRs.  Often it involves quantifying the levels of fit so that alternative solutions can be more easily compared and contrasted.  Software tools are sometimes used to support particular analysis methods, such as ATAM and SARM.  This is typically conducted as a workshop with stakeholders so that trade-offs, possible mitigations, risks and alternatives can be discussed and understood.  The approach encourages consensus as to the way ahead, and often achieves a recognition that there is no solution that can accomplish every requirement to perfection -- a valuable exercise in setting realistic expectations ahead of a major project.

The total time involved depends much on the nature and scope of the system or service being considered.  The "nesting" of architectural patterns within architectural patterns mentioned earlier means that it is possible to apply architecture analysis at different levels, looking at alternative component architectures, collections of components, complete business IT systems and even entire business services that encapsulate multiple business systems.  The process outlined above can occupy anything from a few hours to many days spread out over a number of weeks depending on the level and complexity of the systems and services under consideration.

**Going beyond the basics**

The description above provides a good overview of the basic approach that can help architects and stakeholders together understand how well an architecture fits the requirements, giving valuable insights that can contribute to architectural decisions.  There are a number of areas where one can go a bit further, gaining greater insight that can really help contribute to a major decision about a large or complex system or service.

**Looking beyond quality attributes**

So far we have made the rather dangerous assumption that architectural significance equates to the subset of requirements (often rather sadly referred to as "non-functional requirements") that can be linked to quality attributes.  As [this article](requirements.md){:target="_blank"} makes clear, there are architecturally significant requirements other than those that impact managed quality attributes.  Shouldn't these also be reflected in the trade-off analysis, as they may also be impacted by the trade-offs, risks and compromises inherent in individual solution options?

Do not be tempted to add in all of the requirements that relate to functional suitability, as this risks drowning out the significant ones and losing the benefit of abstraction that has been achieved by focusing on quality attributes.  Instead, consider extending the quality model, perhaps with a separate layer, to additionally consider the key relevant business capabilities.  This might have the effect of extending the scope of the analysis beyond an IT system to a business service, where the ways in which business capabilities are deployed, combining people, processes and technology, can be considered to be architecturally significant alongside those requirements that can be linked to quality attributes.  The analysis becomes one that is considering more fully the set of architecturally significant requirements and might be more appropriately described as an analysis of service architecture.

**Seeing the problem through the eyes of stakeholders**

The value of engaging stakeholders in the analysis process has been rightly emphasized, but the analysis workshop described above focuses on analyzing the trade-offs among the attributes of the quality model (or the quality and capability model if the above extension has been adopted).  If the interests of the stakeholders have been captured in terms of the ASRs they care most about, it is also possible to analyze the trade-offs and differences between solution options from the different perspectives of the stakeholders.  Understanding that a preferred architecture might leave one key stakeholder somewhat unsatisfied might not lead to a different architectural decision, but it can inform a project's communication strategy and might help to ensure that a stakeholder doesn't also become an enemy.  The price for being able to do this additional analysis comes from having to capture detailed information concerning the ASRs that are of most interest to each stakeholder.

**Architecture Review Boards**

Long considered a top-down approach to architecture analysis, actual ARBs are much more dynamic and cross-cutting depending on the Safety & Liability level of the product/project and architecture practice. ARBs are a lifecycle technique used in governance aspects of the architecture practice where formal or informal architecture analysis occurs. This may include a detailed multi-stakeholder review or be peer to peer. The BTABoK is primarily based on three formal methods of analysis which can be used to differing degrees of rigor. The ATAM from the SEI, the PBAAM from Iasa, and the newer SARM method which to a degree replicates the effectiveness of ATAM. Other analysis methods are being cataloged in the next version of the BTABoK.

**Considering value**

Underlying the analysis approach described in this article is a recognition that for any given business problem there may be multiple solutions that address the requirements well, but there is unlikely to be one that addresses them all perfectly, and that different architectures represent different trade-offs among the competing ASRs and their associated quality attributes and business capabilities.

Many of the ASRs are likely to be associated with the ability to realize benefits, either financial or non-financial.  If some solution options will satisfy some ASRs less well than others, it follows that some of the potential benefits will fail to be realized (or at least realized "less well").  Capturing benefits, both financial and non-financial, and associating them with the ASRs, allows the trade-off analysis to consider the differing impacts of alternative architectures on anticipated benefits.  And if the cost of those architectures is known, or can at least be estimated, then in addition to understanding the architectural implications of alternative architectures, the analysis can also point to their likely cost, benefit and value implications.

Gaining this insight as part of architecture analysis comes at a price, rather as it does for the stakeholder perspectives described above.  There may be one hundred or so ASRs, and each one may be associated with financial or non-financial benefits.  If these can be articulated, a tool that supports the architecture analysis can also provide a cost benefit analysis of each solution option and show the trade-offs associated with each option from both financial and non-financial benefit perspectives.  The Cost Benefit Analysis Method (CBAM) extends ATAM into this space, and the SARM tool incorporates this concept to deal with both financial and non-financial benefits, linking them to its risk-oriented views of alternative architectures.  But it requires effort to capture and link the benefit information in order to gain the insights these perspectives can bring.

**The benefits of the architecture analysis**

This article opened with the proposition that architecture analysis can determine how well an architecture meets its primary purpose: to "provide a framework in which to satisfy the requirements and serve as a basis for the design".  Along the way, we have uncovered many additional benefits that can be derived from conducting such analyses.  Among them are:

-   Bringing the stakeholders together, getting them all "on the same page", and helping them to better understand each other's perspectives;
-   Setting realistic expectations for what can be delivered in practice.  It is highly likely that there is no perfect solution to a complex set of business requirements;
-   Anticipating the reaction of different stakeholder groups to each candidate architecture;
-   Developing a robust cost-benefit analysis and understanding how the value proposition changes with different architectures;
-   Understanding the strengths and weaknesses of an architecture, seeing where residual risks lie and enabling architects to plan for anticipated problem areas;
-   Supporting a procurement process by injecting it with architectural thinking;
-   Providing the evidence and arguments to support architecturally significant decisions.  This can be used to demonstrate good decision governance to stakeholders, which might include colleagues, customers, executives, directors, partners and regulators.

This last point highlights the fact that the analysis provides evidence, but no tool should make architecturally significant decisions.  These should remain in the hands of those who are accountable.  Do not hide behind a spreadsheet or a model and be careful to craft your communications from the analyses and their accompanying tools.  This should appeal to the architect as communicator and storyteller.  Behind every architecture analysis lies a story, and it is the job of the architect to find that story and tell it in ways that will not just convince their fellow architects and engineers, but all of their stakeholders.

I'll conclude with perhaps the most important thing to keep in mind when conducting architecture analysis.  The "right" architecture is not necessarily the one with the highest total utility or the lowest aggregate risk score.  It is almost certainly the one that exhibits the most elegance and beauty, and whose residual risks can be most easily mitigated.  Marco Vitruvius Pollio included *Beauty* as one of his three "architectural universals" along with *Utility* and *Firmness*, Christopher Alexander has described his lifelong pursuit of "The Nature of Order", and in his keynote address at the ACM Symposium on Applied Computing in San Antonio on 1^st^ March 1999, Edsger Dijkstra said:

*"After more than 45 years in the field, I am still convinced that in computing, elegance is not a dispensable luxury but a quality that decides between success and failure."*

You cannot outsource your accountability for making an architectural decision to the analysis or its tool.  They are there to shine a light on architectures from many different angles so that you can more easily see both their beauty and their flaws.  Architecture analysis won't make the decision for you, but it will give you that most powerful property, confidence.

# References and Further Reading

Alexander, Christopher, *A Pattern Language: Towns, Buildings, Construction* (New York: OUP USA, 1978), *The Nature of Order*, 1 edition (Berkeley, Calif: Center for Environmental Structure, 2005)

Barbacci, Mario, Mark H. Klein, Thomas A. Longstaff, and Charles B. Weinstock, *Quality Attributes* (Software Engineering Institute, Carnegie Mellon University, December 1995)

Bengtsson, P., and J. Bosch, 'Architecture Level Prediction of Software Maintenance', in *Software Maintenance and Reengineering, 1999. Proceedings of the Third European Conference On*, 1999, pp. 139--47 [https://doi.org/10.1109/CSMR.1999.756691](https://doi.org/10.1109/CSMR.1999.756691){:target="_blank"}, 'Scenario-Based Software Architecture Reengineering', in *Software Reuse, 1998. Proceedings. Fifth International Conference On*, 1998, pp. 308--17 [https://doi.org/10.1109/ICSR.1998.685756](https://doi.org/10.1109/ICSR.1998.685756){:target="_blank"}

Clements, Paul, Rick Kazman, and Mark Klein, Evaluating Software Architectures: Methods and Case Studies* (Addison Wesley, 2001)

Duenas, J. C., W. L. de Oliveira, and J. A. de la Puente, 'A Software Architecture Evaluation Model', in *Proceedings of the Second International ESPRIT ARES Workshop* (Las Palmas de Gran Canaria: Springer, 1998)

Field, Simon, 'Can Software Architecture Review Methods Apply to Service Design?', in *IESS 2010* (presented at the IESS 2010, Geneva: Springer-Verlag, 2010), pp. 111--24

IEEE, 'ISO/IEC/IEEE Systems and Software Engineering -- Architecture Description', ISO/IEC/IEEE 42010:2011(E) (Revision of ISO/IEC 42010:2007 and IEEE Std 1471-2000)*, 2011, 1--46 
[https://doi.org/10.1109/IEEESTD.2011.6129467](https://doi.org/10.1109/IEEESTD.2011.6129467){:target="_blank"}

International Organization for Standardization, *ISO/IEC 9126 -- Software Engineering Product Quality* (International Organization for Standardization, 1991), ISO/IEC 25010:2011 Systems and Software Engineering -- Systems and Software Quality Requirements and Evaluation (SQuaRE) -- System and Software Quality Models* (International Organization for Standardization, 2011)

Kazman, Rick, Gregory Abowd, Len Bass, and Mike Webb, 'SAAM: A Method for Analyzing the Properties of Software Architectures', 1994

Kazman, Rick, Mark Klein, and Paul Clements, *ATAM: Method for Architecture Evaluation* (Software Engineering Institute, Carnegie Mellon University, August 2000)

'List of System Quality Attributes', *Wikipedia*, 2020 
[https://en.wikipedia.org/w/index.php?title=List_of_system_quality_attributes&oldid=953823877](https://en.wikipedia.org/w/index.php?title=List_of_system_quality_attributes&oldid=953823877){:target="_blank"} [accessed 28 May 2020]

Marcus Vitruvius Pollio, *De Architectura*, 25AD

Perry, Dewayne E., and Alexander L. Wolf, 'Foundations for the Study of Software Architecture', SIGSOFT Softw. Eng. Notes*, 17.4 (1992), 40--52 [https://doi.org/10.1145/141874.141884](https://doi.org/10.1145/141874.141884){:target="_blank"}

'SARM Tool Download' 
[https://sarm.org.uk/download/](https://sarm.org.uk/download/){:target="_blank"} [accessed 29 May 2020]

'Solution Architecture Review Method' 
[https://sarm.org.uk/](https://sarm.org.uk/){:target="_blank"} [accessed 28 May 2020]

Szwed, Piotr, Igor Wojnicki, Sebastian Ernst, and Andrzej Glowacz, 'Application of New ATAM Tools to Evaluation of the Dynamic Map Architecture', 2013, ccclxviii 
[https://doi.org/10.1007/978-3-642-38559-9_22](https://doi.org/10.1007/978-3-642-38559-9_22){:target="_blank"}

Wolman, David, 'Before the Levees Break: A Plan to Save the Netherlands', 2008 
[http://www.wired.com/science/planetearth/magazine/17-01/ff_dutch_delta?currentPage=all](http://www.wired.com/science/planetearth/magazine/17-01/ff_dutch_delta?currentPage=all){:target="_blank"} [accessed 20 February 2010]

Dewayne E. Perry and Alexander L. Wolf, 'Foundations for the Study of Software Architecture', *SIGSOFT Softw. Eng. Notes*, 17.4 (1992), 40--52 (p. 43) 
[https://doi.org/10.1145/141874.141884](https://doi.org/10.1145/141874.141884){:target="_blank"}

IEEE, 'ISO/IEC/IEEE Systems and Software Engineering -- Architecture Description', *ISO/IEC/IEEE 42010:2011(E) (Revision of ISO/IEC 42010:2007 and IEEE Std 1471-2000)*, 2011, 1--46 (p. 9) 
[https://doi.org/10.1109/IEEESTD.2011.6129467](https://doi.org/10.1109/IEEESTD.2011.6129467){:target="_blank"}

Christopher Alexander, *A Pattern Language: Towns, Buildings, Construction* (New York: OUP USA, 1978).

Mario Barbacci and others, *Quality Attributes* (Software Engineering Institute, Carnegie Mellon University, December 1995).**

Rick Kazman and others, 'SAAM: A Method for Analyzing the Properties of Software Architectures', 1994.**

Paul Clements, Rick Kazman, and Mark Klein, *Evaluating Software Architectures: Methods and Case Studies* (Addison Wesley, 2001), p. 211.**

P. Bengtsson and J. Bosch, 'Scenario-Based Software Architecture Reengineering', in *Software Reuse, 1998. Proceedings. Fifth International Conference On*, 1998, pp. 308--17 
[https://doi.org/10.1109/ICSR.1998.685756](https://doi.org/10.1109/ICSR.1998.685756){:target="_blank"}

P. Bengtsson and J. Bosch, 'Architecture Level Prediction of Software Maintenance', in *Software Maintenance and Reengineering, 1999. Proceedings of the Third European Conference On*, 1999, pp. 139--47
[https://doi.org/10.1109/ICSR.1998.685756](https://doi.org/10.1109/ICSR.1998.685756){:target="_blank"}

J. C. Duenas, W. L. de Oliveira, and J. A. de la Puente, 'A Software Architecture Evaluation Model', in *Proceedings of the Second International ESPRIT ARES Workshop* (Las Palmas de Gran Canaria: Springer, 1998).

Rick Kazman, Mark Klein, and Paul Clements, *ATAM: Method for Architecture Evaluation* (Software Engineering Institute, Carnegie Mellon University, August 2000).

'List of System Quality Attributes', *Wikipedia*, 2020
[https://en.wikipedia.org/w/index.php?title=List_of_system_quality_attributes&oldid=953823877](https://en.wikipedia.org/w/index.php?title=List_of_system_quality_attributes&oldid=953823877){:target="_blank"}

International Organization for Standardization, *ISO/IEC 9126 -- Software Engineering Product Quality* (International Organization for Standardization, 1991).

International Organization for Standardization, *ISO/IEC 25010:2011 Systems and Software Engineering -- Systems and Software Quality Requirements and Evaluation (SQuaRE) -- System and Software Quality Models* (International Organization for Standardization, 2011).

David Wolman, 'Before the Levees Break: A Plan to Save the Netherlands', 2008
[http://www.wired.com/science/planetearth/magazine/17-01/ff_dutch_delta?currentPage=all](http://www.wired.com/science/planetearth/magazine/17-01/ff_dutch_delta?currentPage=all){:target="_blank"}

'Solution Architecture Review Method'
[https://sarm.org.uk/](https://sarm.org.uk/){:target="_blank"}

Piotr Szwed and others, 'Application of New ATAM Tools to Evaluation of the Dynamic Map Architecture', 2013, ccclxviii
[https://doi.org/10.1007/978-3-642-38559-9_22](https://doi.org/10.1007/978-3-642-38559-9_22){:target="_blank"}

'SARM Tool Download'
[https://sarm.org.uk/download/](https://sarm.org.uk/download/){:target="_blank"}

Simon Field, 'Can Software Architecture Review Methods Apply to Service Design?', in *IESS 2010* 
(presented at the IESS 2010, Geneva: Springer-Verlag, 2010), pp. 111--24.

'SARM Tool Download'.

Marcus Vitruvius Pollio, *De Architectura*, 25AD.

Christopher Alexander, *The Nature of Order*, 1 edition (Berkeley, Calif: Center for Environmental Structure, 2005). By Simon Field

![image001](media/by-nc.png)

BTABoK 3.0 by [IASA](https://iasaglobal.org/) is licensed under a [Creative Commons Attribution-NonCommercial 4.0 International License](http://creativecommons.org/licenses/by-nc/4.0/). Based on a work at [https://btabok.iasaglobal.org/](https://btabok.iasaglobal.org/)

