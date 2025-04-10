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

Alternatively, GitHub Desktop can be used to clone the repository to your local computer and work with content locally. GitHub Desktop keeps track of the files that are changed and when the content is ready for commit, all the changed files can be committed. However, merge conflicts will have to managed manually.

## Commit Changes to Candidate branch

When the content in the contribution branch is ready for review it can be committed to the candidate branch in preparation for publishing. In order to commit content to the candidate branch a pull request is created.

The following process is used:

1. Select the contribution branch
2. Select **Compare & Pull Request**
3. Select **base:candidate** as the branch to merge to
4. Add a description for the Pull Request
5. Click **Create Pull Request**

A Pull Request is created and will show if there are any conflicts with the changes on the candidate branch. An editor can be given as a reviewer and if there are no conflicts the changes can be merged to the candidate branch by selecting **Merge Pull Request**.

If there are many commit items in the pull request there is the option to **Squash And Merge**, which squashes the commit items into a single commit, this can make the branch history more manageable.

## Updating Contribution branch from Candidate

Other teams and individuals will be working with content on their own contribution branches and committing their work to the candidate branch. In order to keep a contribution branch updated, the contributors will want to update their own contribution branch with new content from the candidate branch.







