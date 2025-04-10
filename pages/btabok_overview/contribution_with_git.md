---
title: "Contribution With GIT"
keywords: 
sidebar: mydoc_sidebar
toc: true
permalink: contribution_with_git.html
folder: btabok_overview
summary: "Instructions and help for contributing content with GIT."
tags: 
  - git
---

# Contributing to BTABoK with GIT

The BTABoK uses GIT as a content control repository to ensure that individuals and teams can work with which is a work-in-process, while editors can help with quality control and coordinated publishing of content.

In order to do this there are three types of branches in the BTABoK repository:

- contribution/<name> - branches which teams or individuals actively work and change content
- candidate - the branch where editors work to co-ordinate and provide quality assurance for the contributions from teams and individuals
- main - the branch which which contains the final publishable content



# Contribution Branch

## Creating the branch

Teams and individuals can create a **contribution** branch using the name format "contribution/<contribution_name>". The branch shall be created from the **candidate** branch, this way the contributors will be informed of changes in the candidate branch which can be merged with their contribution branch.

Contribution branch can be created with the following steps in GitHub web:

1. Switch you active branch to **candidate**
2. In the "branch" drop down box, type the name of your new branch, e.g. contribution/architecture_stuff
3. Notice the "Create" option in the menu shows "Create branch **contribution/architecture_stuff** from **candidate**."
4. Click this option to create the branch and the new branch is available

## Adding and Changing Content

In order to add content to the branch there are a number of options. Contributors can work with a local repository using an application such as GitHub Desktop, or work directly with the web interface on GitHub.

Using the web interface contributors can open any markdown file and edit the content and then commit the content to the branch. A commit is made for each change to each file using the option to **commit directly** to the branch.

Alternatively, GitHub Desktop can be used to clone the repository to your local computer and work with content locally. GitHub Desktop keeps track of the files that are changed and when the content is ready for commit, all the changed files can be committed and merged with changes that other contributors have committed.







