The Business Technology Architecture Body of Knowledge (BTABoK) is a free public archive of Business Technology architecture best practices, skills, and knowledge developed from the experience of individual and corporate members of Iasa, the world’s largest architecture professional organization.  

You can find the BTABoK github pages site at: [BTABoK (iasa-global.github.io)](https://iasa-global.github.io/btabok/)

BTABoK provides the tools and resources needed by individuals and organizations to set industry standards for professional career development and well as hiring practices and incorporation of IT architects into established or developing institutions.

![](media/311ca0bebe2188ba201da0e9211ff2ddf0acacad.svg)

## Who is the BTABoK for?

The BTABoK was designed ground up to be a practical resource for any type of architect in any type of organization. It includes as much business as technical thinking as well as up to date tools in both of these spaces. It has a very strong approach to stakeholder management as well as an easy to use competency model which can be modified for your organization.

## What is in this Site?

The BTABoK is a tool. It works for all architects whether you consider yourself a business focused architect or a technical one. It is also the only truly open body of knowledge in existence. In the following video Paul Preiss describes the value and the use of the BTABoK (he uses it's previous title, ITABoK but they are the same thing). 

https://user-images.githubusercontent.com/41272798/187097260-027cc44a-86e8-4d17-bc25-b22ef527de22.mp4

**Defining the IT Architect Profession** – What is a BT architect? We provide industry reference models for architects skills and competencies backed by international certifications.

**Utilization & Engagement of IT Architects** – How are IT architects utilized within organizations and what are the interaction models between them and their clients or employers?

**Career Pathway** – Describes the standard career path of an architect including specializations and career achievement milestones.

## Overview

The Business Technology Architecture Body of Knowledge (BTABoK) has been developed from the experience and practice of individual and corporate members.

In addition to being a reference, a knowledge base and a list of professional capabilities, the BTABoK is meant to be essential in implementing an architecture practice within an organization, without significant changes to other standards, roles, practices and lifecycles. An architecture practice provides high levels of value in both business and technical strategy, and that value can be measured as a contribution to the organization. Architecture is appropriate and essential for extremely small businesses, as well as, the largest businesses in the world, including non-profit, government, and defense.

The BTABoK is first and foremost intended for individual practicing architects, though it does include significant portions dedicated to organizational excellence. It is meant as a people framework as opposed to a process, methodology or standard. It is meant to be the living body of knowledge for the practice of an architect attempting to fulfill their duty to their customer or employer. While Iasa includes corporate examples and concerns, the BTABoK must be useful by the independent practitioner and must assume that a single architect is as important as a group of architects. In addition, the BTABoK must be consistent and useful at any degree of scale, regardless of the number of architects involved in the endeavor, whether that be the delivery of a global fortune 100 business strategy or the delivery of a single solution for a small business.

The BTABoK is inclusive of all specializations, sub-specializations and career levels of the architect profession. Although the title includes the term information technology, the content has been written by keeping business, enterprise, solutions, software, information and infrastructure architects and their derivations in mind. Practitioners from each of these specializations continue to help in the development and maintenance of the body of knowledge.

## What is Architecture

As the favorite topic of architects everywhere, what is architecture and what are architects is central to the theme of the BTABoK. Read the [What is Architecture Article](/pages/btabok_overview/what_is_architecture.md). 

## Roadmap

The plan is to have version 3.0 as the main branch by the end of the summer. From here we will create a new branch for version 4.0 which we expect to freeze next summer. The main goals of version 4.0 are to:

- Rework and modernize the competency model
- Develop a further connection with engineering and other architect partners
- Create a complete set of deliverables using the BTABoK
- Complete the patterns library and other libraries of the BTABoK

## Committers and Editors

The BTABoK is the only truly open source and maintained body of knowledge for architects. As an open source BoK anyone can do a pull request after fixing or suggesting changes to the BTABoK or adding material. The committers on the project are a group of board certified architects who have worked very hard to create the body of knowledge. They will determine what pull requests get included into the BTABoK. To become a committer you will have to have a large number of successful pull requests and have a discussion with the committer team.

### BTABoK Editing Guidelines

The BTABoK is designed with a theme, linking and embedding primarily targeted at the BTABoK GitPages site. However, it also serves in many other functions. Thus it is important to follow the guidelines in editing the body of knowledge. Any pull requests that do not will be rejected.

The major elements of the guidelines include

- How to write BTABoK Articles – Writing Guidelines (separate link)
- Markdown Editors – The committers primarily use MarkText or Word with an addon called Writage (<https://www.writage.com/>). However as long as it is valid markdown using simple formatting it is up to the author what to use.
- Images – standard images should be stored in the media folder in png format. The images must be licensed for free use or created by the author of the article and express permissions put in the GitHub ‘add’ comments. This frees us from concern over image licensing issues.
- Canvases – canvases and cards should be stored in two primary formats – ppt and SVG. This makes the editing of canvases relatively easy for anyone in the world as well as making them usable to architects doing presentations. These should be stored in media/canvases for the SVG files and media/files for the ppt files (the SVG files are considered the master copy).
- Linking – linking should always be relative within the BTABoK as the files are published to gitpages. However, the goal is to convert these to published files on the official WordPress pages as well. This will be covered in a separate section.


# Introduction

The following guidelines are intended for use when writing
articles for the ITABoK 3.0. The aim of the guidelines is to support authors in
writing articles to a similar structure and writing style.

In the following sections the term “Subject Matter” is used
to refer to the subject being described by an author in an article.

# Writing Style

Articles for the ITABoK are written in third-person form
which is commonly used in academic texts.

“Writing in [third
person](https://www.yourdictionary.com/third-person#websters) is writing from
the third-person point of view, or outsider looking in, and uses pronouns like
he, she, it, or they. It differs from the [first
person](https://examples.yourdictionary.com/examples/examples-of-writing-in-first-person.html), which uses pronouns
such as I and me, and from the [second
person](https://examples.yourdictionary.com/reference/examples/examples-of-writing-in-second-person.html), which uses pronouns
such as you and yours.” - **YourDictionary.com**

It is also preferable to provide use the noun (or the role
of the person, architect, stakeholder, consumer) rather than using the pronoun
“he” or “she” in order to avoid gender issues.

# Basic Article Structure

Articles can sometimes vary in structure due to the nature
of the subject matter. However, the following provides a basic generic
structure.

## What is “The Subject Matter”

The first section in the article gives a brief description
of what the subject matter is. Standard definitions or quotes may be used to
support this section. The aim of this section is to ensure that the reader
understands what the “Subject Matter” is before reading the rest of the
article. This can also be important since certain “Subject Matters” can be
discussed in different contexts, this section provides the opportunity to set
the “Subject Matter” in context.

```
**For example:  
**A roadmap is a visual description which shows a plan against time for
achieving one or more goals or objectives.
```

## Why we need “The Subject Matter”

The second section of the article describes why we need the
“Subject Matter” or why the “Subject Matter” is important. Before discussing
deeper concepts or practices it is important that the reader understands why
the “Subject Matter” in real terms. Describe the key benefits of addressing the
“Subject Matter” or the negative effects if the “Subject Matter” is not
addressed.

```
**For example:  
**Roadmaps are important as they provide a common understanding for
stakeholders regarding the current status of a business initiative and
also a broad plan for future deliverables, goals and objectives.
```

## “Subject Matter” Approach

The third section lists a set of key factors which are
considered important when approaching the “Subject Matter”. These key factors
are expressed as small sections with a memorable statement as a title.

```
**For example:**  
“Plan the Journey”,  
“Monitor the technical debt”,  
“Start small, scale fast”.
```

This provides the reader with an overview of the key factors
in the “Subject Matter” and the statement as a title should make these factors
more memorable to the reader. The reader and the author can also reflect on
these key factors in the “Concepts and Practices” sections of the article where
practical examples can be given.

## Concepts

The concepts of the “Subject Matter” can be described in a
series of sections which describe important areas of the “Subject Matter”. The
structure and naming of the concept sections will vary depending on the
“Subject Matter” and how the author wants to present the “Subject Matter” to
the reader. It is important when writing the concept sections that the reader
feels that the sections flow from one to the other and that knowledge is gained
step by step.

One technique is to create an overview concept which links
the following concept sections so the reader understands how the different
concept sections are connected.

Another technique is to start the concept at an abstract
level and use a “top-down” description describing the concept in more detail as
the author moves down the sections.

## Techniques and Canvases

When describing concepts practical advice may be provided by
the author regarding how to work with the “Subject Matter”. This may involve
providing a canvas or a technique which will help the reader to actively work
with the “Subject Matter”. When describing how to use a canvas or a technique
the following structure may be useful.

1.       Provide a short text describing why the technique
or canvas is useful

2.       Describe any preparation that that should be
done before starting

3.       Describe in sequential steps (Step1, Step2,
Step3….) how the reader uses the technique or canvas

The description of a technique or canvas can be described as
part of concept section, where the technique or practice is directly related to
the given concept. However, they can also be provided as separate sections as
appropriate.

## Add or edit images to our repositoriy

1. Only images in .png or .svg format will be accepted.
2. The images will have to be added to the folder that has the name media.
3. What name is given to the file?
    - We name the image file with the same name as the file we are editing, only we add the consecutive number. Example: xyz.md is the file to edit, the image file would be xyz01.png
4. Label to display the image: 

```
![](media/name_of_the_image_01.svg) or ![](media/name_of_the_image_01.png)

```

## References and Further Reading

At the end of each article there should be a section for
“References and Further Reading” which contains a list of books, articles or
texts which have been used in constructing the article, or which are useful to
the reader for further reading on the “Subject Matter”.

## Additional Help Needed

We are also looking for committers to help develop and extend the functionality of the site. For example, we would like to commit automatically to wordpress from this site so that it is always up to date. 
