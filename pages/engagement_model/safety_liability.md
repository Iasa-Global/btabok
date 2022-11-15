---
title: "Safety & Liability"
keywords: 
sidebar: mydoc_sidebar
toc: true
permalink: safety_liability.html
folder: engagement_model
summary: "Like any tool, software can be misused, or used for a purpose for which it was not intended (ever use a screwdriver as a chisel or prybar?)."
tags: 
  - digital_operations
---

> "It takes leadership to improve safety."
**Jackie Stewart**

# Introduction

Surprisingly, safety doesn't appear on any of the lists of quality attributes and is rarely mentioned in relation to software systems, yet it is one of the most important. In 1997, a definition of software engineering was published that explicitly mentions safety as a major criteria for the success of a software system:

*Software engineering is the science and art of designing and building, with economy and elegance, software systems and applications so they can safely fill the uses to which they may be subjected.*

There is a lot embedded in this definition, but we'll focus on the last phrase: "...so they can safely fill the uses to which they may be subjected." The implication here is that software should be safe to use. Used for its intended purpose, it should just work. Period. Beyond that, use of the software should do no harm; it should not damage anything, including information, property, or the reputations of its builders or users.

Like any tool, software can be misused, or used for a purpose for which it was not intended (ever use a screwdriver as a chisel or prybar?). In these cases, the software should either accommodate the use, or safely resist it.

Failures happen, either because of errors in the software or conditions in the environment. When the software cannot recover from or work around such a condition, it should fail gracefully and safely.

Iasa Global has adopted the position that the safety of a software solution is the responsibility of the architect who designed it; the architect is professionally liable for any safety related failures that are due to their own errors or negligence. The notion of professional liability is new to most software people, but Iasa Global believes that only when architects step up and accept it will architecture truly be a profession.

This article explores safety as a quality attribute of software-based solutions. We classify applications into three tiers, each requiring a different level of safety and perhaps different [risk](risk_methods.md){:target="_blank"} analysis methods and tests. Finally, we describe a safety framework including professional qualifications, codes of ethics, licensure, standards, and enforcement.

As software becomes more complex and is asked to do more, failure will have increasingly severe consequences. Iasa Global believes that our architects are in the best position to ensure the safety of software-based solutions both technically and to the public.

# Safety In Software-Based Solutions

## What is Safety?

Simply put, safety as a [quality attribute](quality_attributes.md){:target="_blank"} means that a software-based solution, or any solution that contains software, includes the prevention of adverse events arising from normal or abnormal use and protections from harm when they do. When used as intended, a safe software system will not fail under normal conditions, and will fail gracefully when those conditions are violated. In addition, a safe system will resist being used in an unsafe manner when possible, or at the very least, prevent or limit any harm as a result of such use. A system should do no harm to people or property, including to the reputations of its builders and users.

Safety includes the absence of defects, but it goes much further. Since it is not possible to guarantee that software is free from defects, measures must be taken to ensure that any failures are graceful, that is, relatively harmless.

To make a system safe, the architect must identify, assess, and mitigate risks that can lead to system failure and risk that result from system failures. Dealing with risk is the subject of another article; here, we focus on the level of rigor required when analyzing risk.

With all of that, it is not possible to guarantee that catastrophic failures will not occur; airplanes still crash, buildings and bridges still collapse, yet most are considered safe. A commercial jet engine typically fails once per one million hours of operation. Buildings and bridges fail much less often (and most of those are due to combinations of outside factors). A safe software system is one in which a catastrophic failure either requires external factors, such as a natural disaster, or occurs only very rarely.

## Safety Tiers

The level of safety required in a system is a function of the application, which we group into three tiers based on the severity of consequences of failure.

## Tier 1

Tier 1 systems are those that have been classically defined as safety-critical. Consequences of failure in such systems result in loss of life, injury, loss of or damage to equipment, or damage to the environment. Placing someone in a situation where they risk death or injury, such as loss of power during a heat or cold snap, also places a system in Tier 1. Rigorous risk analysis methods, such as Fault or Functional Hazard Analysis (FHA), Fault Tree Analysis (FTA), Failure Mode Effects and Criticality Analysis (FMECA), or Software Hazard Analysis (SHARD), should be used. Other methods of analysis and specifications for testing and review might be required by law, regulation, or common practice.

## Tier 2

The consequences of failure in a Tier 2 system do not rise to the level of Tier 1, but include large financial losses, such as recovery costs, loss of revenue, or the payment of ransom. Examples include disruption of service in a commercial website, airline reservation system, or the billing system for a mobile phone carrier. A data breach in which unencrypted personal identifying information (PII) is released also puts an application into tier 2. Rigorous application of a method such as Fault Tree Analysis should be used to identify risks, and the [design](design.md){:target="_blank"} must include mitigation for each identified risk. Review and testing methods are left to the client organization.

## Tier 3

The most severe consequence of failure for a system in Tier 3 is inconvenience or loss of use. The user is not at risk of personal harm or loss of information. Recoverable data falls into this tier as well; that is, loss of data is tolerated if the data is recoverable within a reasonable timeframe, specified by the client. Standard software failure analysis, review, and testing are sufficient for these systems as failures are more annoying than harmful.

# Professionalism and Liability

The concept is simple: you cannot consider yourself a professional unless and until you assume responsibility for the consequences of someone being harmed by the results of your work due to error or negligence on your part. Errors and negligence can include both acts of commission (what you did) and acts of omission (what you didn't do). Errors are typically accidental, while negligence arises from deliberate action. There are exceptions to this, but in the main, you are responsible for the safe performance of your work. In practice, this means that if you can foresee a harmful use of your work, you must do what you can to prevent it, unless doing so renders your work unfit for its intended purpose. This is a fine line fraught with twists and turns and seemingly unintuitive outcomes. A brief look at professional and product liability law should convince you.

This section, while not valid as legal theory, sets the direction to establish a framework for assuming professional liability for the safety of the products we architects produce. Actual cases and actual trials will alter this direction, but setting it now gives us a better chance to influence the final outcome.

The proposed framework includes minimum standards for training and certification of people as professional architects, a code of ethics, and may include licensing requirements. Minimum standards for the safety of a software-based solution is based on the tier of the risk and the consequences of safety failures and is driven by legislation and regulation. Enforcement of all of these requires legislation, regulation, and a strong professional society dedicated to the self-regulation of practicing professionals, regardless of membership.

# A Framework for Safety

## Code of Ethics

The professional (and sometimes personal) behavior of the members of every profession is governed by a code of ethics created and published by a professional organization. These codes generally lay out the minimum standards for professional practice and include penalties for violations. Iasa Global is working on a code of ethics for technical architects.

## Professional Qualifications

Qualification to practice a profession requires significant learning, both academic and guided experience. Passing an exam and/or peer review is required evidence of qualification, which may take the form of certification in a market-based situation, or licensure when required by statute.

## Certification

Clients, insurers, and the public (governments) have an interest in making sure that only qualified professionals design systems in Tiers 1 and 2, at least. To protect these interests, they may require that architects certifying such systems have a specific type or level of certification, such as Iasa Global's CITA-P or The Open Group's Certified Architect at that Master level (level 2). These particular certifications, as well as others, are based on bodies of knowledge and peer review of evidence of past practice of architecture. The standards for certification are maintained by the respective organizations, and those who require these certifications rely on the organizations to maintain the meaningfulness and value of the certification.

## Licensure

Some jurisdictions may further require that architects also be licensed. Professional licensing is a powerful tool for enforcing codes of ethics and standards of professional conduct. Many professions require a license to practice, including building architects. Licensure of software and solution architects might be a good way to enforce safety in software applications.

## Codes and Standards

Given the risks involved in some kinds of software, jurisdictions and some large clients (such as the Department of Defense) might create and impose codes and standards similar to building codes. These codes and standards would specify minimally required processes for identifying and mitigating risks associated with systems in Tier 1, and maybe Tier 2. Standards may also specify techniques to be used to minimize the risk or loss from an event, and at the very least specify minimum levels of testing and performance.

## Enforcement

Three main mechanisms exist to enforce compliance with codes of ethics and standards: higher liability insurance premiums, loss of certification and/or license, and civil and/or criminal penalties.

## Insurance Premiums

Professionals generally take out policies to cover errors and omissions that may happen in the course of their work. No matter how careful one is, errors happen, and insurance covers any costs associated with making whole the injured parties. Frequent use of such insurance will cause rates to raise. In addition, insurers might require a minimum level of certification or license to grant coverage or charge preferential rates.

Professional liability insurance typically does not cover results of gross negligence, in which the professional acts in willful disregard of the standards of practice or the consequences of his or her actions. A finding of gross negligence can result in the loss of coverage, making it financially impractical to continue to practice. In the absence of licensing statutes, some jurisdictions require that a professional carry professional liability insurance, and loss of coverage can mean that it is illegal to continue to practice, making required coverage effectively equivalent to licensure, but putting the burden for administration and discipline on the insurer rather than a government agency.

## Loss of Certification/Licensure

A certifying association may include in its code of ethics provisions for removal of certification as a disciplinary measure for violating standards of professional practice. Associations maintain a process to review a case and determine a course of action. Government jurisdictions that grant professional licenses also have processes in place to review and make determinations for action when a professional license is involved. Serious infractions of professional practice may involve both actions, the most serious consequence of which is the loss of the right to practice the profession.

## Civil and Criminal Penalties

Serious breaches of standards, practice, or willful violations of law may warrant additional penalties. These can range from fines to jail time depending on the nature of the offense. Such penalties are prescribed by law, so legislation is required to enact them.

# Conclusion

Safety is the forgotten quality attribute. It covers a wide range of aspects related to the performance of software system and the professionals who create them. Iasa Global is proposing a three-tiered classification for safety based on the risks in the application and the severity of the consequences of failure. Our aim is for these tiers to be the basis for legislation and regulation to govern aspects of the software products as well as the practice of professional software and solution architects. We are proposing that clients of tier 1 and tier 2 systems, government agencies, insurers, and the professional community at large work towards requiring a professional license to create and certify systems in those tiers.

# References

**Whitmire, Scott A. *Object-Oriented Design Measurement*, John Wiley & Sons, New York, NY: 1997.**

**"Safety-critical system". encyclopedia.com**
[Safety-critical system](http://www.encyclopedia.com/computing/dictionaries-thesauruses-pictures-and-press-releases/safety-critical-system){:target="_blank"}

**Vincoli, Jeffery W. *Basic Guide to System Safety*, John Wiley & Sons, New York, NY: 2014.**

**Lee, W. S., D. L. Grosh, F. A. Tillman and C. H. Lie, "Fault Tree Analysis, Methods, and Applications ߝ A Review," in IEEE Transactions on Reliability, vol. R-34, no. 3, pp. 194-203, Aug. 1985, doi: 10.1109/TR.1985.5222114.**

**Jordan, Wallace E. "Failure modes, effects and criticality analyses." Annual Reliability and Maintainability Symposium, 1972.**

**McDermid, J. A., M. Nicholson, D. J. Pumfrey and P. Fenelon, "Experience with the application of HAZOP to computer-based systems," COMPASS '95 Proceedings of the Tenth Annual Conference on Computer Assurance Systems Integrity, Software Safety and Process Security', 1995, pp. 37-48, doi: 10.1109/CMPASS.1995.521885.**

**Iasa Global. "Ethical Guidelines".**
[Iasa Global. "Ethical Guidelines"](https://iasa-global.github.io/btabok/ethics_and_principles.html){:target="_blank"}

**Iasa Global. "Training and Certification -- Professional"**
<https://iasaglobal.org/Public/Learn/Certifications/Public/Learn/Training_and_Certifications.aspx?hkey=b18264af-a223-4a2e-a77c-053356d1a486>

**The Open Group, "Certified Architect (Open CA)"**
**<https://www.opengroup.org/certifications/certified-architect-open-ca>

![image001](media/by-nc.png)

BTABoK 3.0 by [IASA](https://iasaglobal.org/) is licensed under a [Creative Commons Attribution-NonCommercial 4.0 International License](http://creativecommons.org/licenses/by-nc/4.0/). Based on a work at [https://btabok.iasaglobal.org/](https://btabok.iasaglobal.org/)