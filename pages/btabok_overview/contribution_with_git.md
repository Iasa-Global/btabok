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

# Contributing To BTABoK With GIT

The BTABoK uses GIT as a content control repository to ensure that individuals and teams can work with which is a work-in-process, while editors can help with quality control and coordinated publishing of content.

In order to do this there are several types of branches/fork in the BTABoK repository:

- fork -  forks are used for public access to the BTABoK, BTABoK GIT account is not required 
- contribution/<name> - branches which teams or individuals actively work and change content
- candidate - the branch where editors work to co-ordinate and provide quality assurance for the contributions from teams and individuals
- main - the branch which which contains the final publishable content



# The Basics

## Adding And Changing Content

Content is added or changed in a branch or a fork. Contributors can work with a local repository using an application such as GitHub Desktop, or work directly with the web interface on GitHub.

Using the web interface contributors can open any markdown file and edit the content and then commit the content to the branch. A commit is made for each change to each file using the option to **commit directly** to the branch option.

Alternatively, GitHub Desktop can be used to clone the repository to your local computer and work with content locally. GitHub Desktop keeps track of the files that are changed and when the content is ready for commit, all the changed files can be committed. However, merge conflicts have to managed manually.

## Creating A Pull Request

When the content in the a branch or fork is ready for commit to another branch (contribution, candidate or main) a pull request is created. This is a request to the merge the changes into a target branch from a  source branch, this may require review by the owners of the target branch before the request is accepted. 

The following process is used:

1. Select the contribution branch
2. Select **Compare & Pull Request**
3. Select **target branch** as the branch to merge to and the **source branch** as the branch with the changes to be comitted
4. Add a description for the Pull Request
5. Click **Create Pull Request**

A Pull Request is created and will show if there are any conflicts with the changes on the candidate branch. 

The contributor then has to wait for the pull request to be accepted, or if contributor has the correct access rights the pull request can be accepted by selecting **Merge Pull Request**.

If there are many commit items in the pull request there is the option to **Squash And Merge**, which squashes the commit items into a single commit, this can make the branch history more manageable.



# Fork

## Creating a Fork

Any team or individual can create a **fork** which is a copy of the repository where changes do not . Content can be changed in the fork without affecting the BTABoK repository. Content can be submitted to the BTABoK repository by creating a pull request to a **contribution** branch.

A fork can be created with the following steps in GitHub web:

1. In GitHub menu select **fork**
2. Choose a name for the fork
3. Then select **Create Fork**

## Committing Changes From A Fork

Changes from a fork are committed to a **contribution** branch in the BTABoK. This is done by creating a pull request from the target branch (fork) to the contribution branch (contribution/<name>).

The owner of the contribution branch will review the pull request and will accept or reject the changes.

# Contribution Branch

## Creating The branch

Teams and individuals can create a **contribution** branch using the name format "contribution/<contribution_name>". These branches are created from the **candidate** branch and can only be created by contributors with the appropriate access rights.

A contribution branch can be created with the following steps in GitHub web:

1. Switch you active branch to **candidate**
2. In the "branch" drop down box, type the name of your new branch, e.g. contribution/architecture_stuff
3. Notice the "Create" option in the menu shows "Create branch **contribution/*architecture_stuff*** from **candidate**."
4. Click this option to create the branch and the new branch is available



## Commit Changes To Candidate branch

When the content in the contribution branch is ready for review it can be committed to the candidate branch in preparation for publishing. In order to commit content to the candidate branch a pull request is created.

When creating the pull request ensure that the target branch is **base:candidate** and the source branch is **base:contribution/<name>** .



## Updating Contribution Branch From Candidate

Other teams and individuals will be working with content on their own contribution branches and committing their work to the candidate branch. In order to keep a contribution branch updated, the contributors will want to update their own contribution branch with new content from the candidate branch.

To update a contribution branch with changes in the candidate branch create a pull request and ensure that the target branch is **base:contribution/<name>**  and the source branch is **base:candidate**.

# Candidate Branch

The candidate branch is managed by BTABoK editors and changes directly to this branch is only possible for users with editor access rights. Changes to candidate branch from contributors is managed through pull requests.

# Main Branch

The main branch is managed by BTABoK editors and changes directly to this branch is only possible for users with editor access rights. Changes to the main branch are only made from a merge with the candidate branch. Only editors have the access rights to merge candidate branch with main branch. 
