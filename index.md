---
title: "Getting started"
keywords: sample homepage
tags: [getting_started]
sidebar: mydoc_sidebar
permalink: index.html
summary: The Business Technology Architecture Body of Knowledge (Btabok) is a free public archive of IT architecture best practices, skills, and knowledge developed from the experience of individual and corporate members of Iasa, the world’s largest IT architecture professional organization.
---

{% include note.html content="This site is currently a working draft." %}

## Welcome to BTABoK Pages

Welcome to the Iasa BTABoK. This is the primary source material for the BTABoK which is converted to maintain the BTABoK Wordpress Site which is our more advanced navigation and content site. The wordpress site includes many addtional tools for members of Iasa such as learning shots and examples.

## Who is the BTABoK for?

The BTABoK was designed ground up to be a practical resource for any type of architect in any type of organization. It includes as much business as technical thinking as well as up to date tools in both of these spaces. It has a very strong approach to stakeholder management as well as an easy to use competency model which can be modified for your organization.

## What is in this Site?

The gitpages version of the site is here: https://iasa-global.github.io/btabok/

The BTABoK repository includes all of the main content for the BTABoK. It is navigable in the same way as the primary BTABoK site.

1. The Engagement Model - includes the articles related to building and managing an architecture practice.
   1. While we are experimenting we have uploaded this articles
      1. [**Design**](pages/design.md) 
      2. [**Requirements**](pages/requirements.md)
      3. [**Requirements Modeling**](pages/requirements_modeling.md)
      4. [**Architecture Pattern Repository**](pages/architecture_pattern_repository.md)
   2. The Structure Canvas Approach is listed as a part of the engagement model. All canvases are being stored in the cavases folder as .svg files which are editable by anyone with an SVG editor.
2. The Competency Model - includes the articles related to architecture competencies
3. The Maturity Model - includes the articles related to understanding architecture practice maturity
4. Lists of useful tools
   1. The BTABoK is capturing many useful tools in addition to the canvases. For example, it includes a pattern library, where we hope to store all of the useful patterns which are vendor neutral. Feel free to add to these libraries where useful.

## Roadmap

The plan is to have version 3.0 as the main branch by the end of the summer. From hear we will create a new branch for 4.0 which we expect to freeze next summer. The goals of 4.0 are to

- rework and modernize the competency model
- develop a further connection with engineering and other architect partners
- create a complete set of deliverables using the btabok
- complete the patterns library and other libraries of the btabok

## Committers and Editors

The BTABoK is the only truly open source and maintained body of knowledge for architects. As an open source bok anyone can do a pull request after fixing or suggesting changes to the bok or adding material. The committers on the project are a group of board certified architects who have worked very hard to create the body of knowledge. They will determine what pull requests get included into the bok. To become a committer you will have to have a large number of successful pull requests and have a discussion with the committer team.

### BTABoK Editing Guidelines

The BTABoK is designed with a theme, linking and embedding primarily targeted at the BTABoK GitPages site. However, it also serves in many other functions. Thus it is important to follow the guidelines in editing the body of knowledge. Any pull requests that do not will be rejected.

The major elements of the guidelines include

- How to write BTABoK Articles – Writing Guidelines (separate link)
- Markdown Editors – The committers primarily use MarkText or Word with an addon called Writage (<https://www.writage.com/>). However as long as it is valid markdown using simple formatting it is up to the author what to use.
- Images – standard images should be stored in the media folder in png format. The images must be licensed for free use or created by the author of the article and express permissions put in the GitHub ‘add’ comments. This frees us from concern over image licensing issues.
- Canvases – canvases and cards should be stored in two primary formats – ppt and SVG. This makes the editing of canvases relatively easy for anyone in the world as well as making them usable to architects doing presentations. These should be stored in media/canvases for the SVG files and media/files for the ppt files (the SVG files are considered the master copy).
- Linking – linking should always be relative within the BTABoK as the files are published to gitpages. However, the goal is to convert these to published files on the official WordPress pages as well. This will be covered in a separate section.

## Additional Help Needed

We are also looking for committers to help develop and extend the functionality of the site. For example, we would like to commit


{% include links.html %}
