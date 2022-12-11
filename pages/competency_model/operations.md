---
title: "Operations"
keywords: 
sidebar: mydoc_sidebar
toc: true
permalink: operations.html
folder: competency_model
summary: "In a properly run environment, all operating systems would be properly operationalized."
tags:
  - infrastructure_architecture
---

# Description

Operating systems provide an abstraction between applications and the physical hardware resources.  Operations architecture ensures that these systems perform as expected by centrally unifying the control of operational procedures and automating the execution of operational tasks. It also reports the performance of the IT infrastructure. The implementation of an operations architecture consists of a dedicated set of tools and processes which are designed to provide centralisation and automation.

# Overview

In the early sixties, the first operating systems came in support of mainframe computers that were designed by IBM. IBM created OS/360, which was an operating system that spanned all the systems in the product family. This was the first instance when a single centralized entity was created to manage all the system processes and resources, where many of the implementations within current operating systems can be traced. For example, operating platforms started out on mainframes, which were large computers that were run by a single operating system. Jobs were entered and scheduled, then executed by the operating platform. As technology advanced, minicomputers started to become more popular and computer processing decentralized. This trend continued for many years, becoming more and more decentralized, until virtualization became advantageous and more popular. Smaller systems gave way to larger ones, that were run by a single operating system. Jobs (virtual guests) are entered and scheduled, then executed by the operating platform.

There are many different types of operating platforms (some of which are combined):

-- Real-time operating system is a multi-tasking system that executes real-time applications

-- Multi-user systems, where multiple users can be accessing a system concurrently

-- Multitasking, where multiple applications can be run concurrently on a single system

-- Distributed, where multiple discrete computers are bound together to act as a single system

-- Embedded, compact operating systems that run within a specific physical framework

# Proven Practices

## Operating Architecture

-   Process Management
-   Interrupts
-   Memory Management
-   File System
-   Device Drivers

**Process Management** are the structures that allow for processes to be created, to interact with one another, and to be isolated from one another during the run-time state. Process management is what allows operating systems to be able to multi-task.

**Interrupts** are methods that allow processes to be able to signal other system resources that they need resource time, such as processor cycles. This orderly method prevents processes from completely dominating system resources and providing a balanced and efficient operating environment. Interrupts can be broken into two categories, hardware and software. A hardware interrupt would be normally directed at the processor, ensuring that a specific process can get the CPU time that it needs. A software interrupt would be instructions within an operating set, which generates context switches. Context switches are the process of storing state of a executed thread, to be later retrieved for future processing. Interesting ancedote, is that when hardware interrupts skyrocket across a system, that generally indicates that a hardware problem exists within the server.

**Memory management** is the act of managing computer memory.

**File system**, is driven through the operating system.

**Device drivers** are used to provide an interface between a physical piece of hardware and the operating system itself. Device drivers are used for nearly every interface, such as a network interface car, a host bus adapter, CD-ROM drives, etc.

## **Hardware Abstraction**

-   A hardware abstraction layer (HAL) is used to give a common presentation of hardware resources to an operating system
-   Resides at the kernel level
-   Virtualization reduces complexity of the HAL
-   Embedded hypervisors

> Hardware abstraction layers (HAL) allow application authors to write to a standard specification to be able to access a hardware device resource, regardless of manufacturer. For example, a network interface card from multiple manufacturers would be address by an application in the same way, through the HAL. This reduces the amount of knowledge that application developers would need about the specifics of how to address hardware.

> The HAL operates within the kernel, which can explain why hardware problems can lead to a variety of unusual issues in other areas of the operating system.

> The need for complicated HALs are reduced through virtualization, which present a uniform and smaller set of physical devices that would be addressed by applications through the operating system. Currently virtualization is accomplished through a software hypervisor, like Microsoft's Hyper-V or VMWare's ESX, but there is a trend coming that will present hypervisors as part of the motherboard or the CPU itself. Thus, all operating systems on these platforms would be virtualized, even in a standalone independent method. Over time, this will allow operating system manufacturers to focus more on performance and functionality, rather than working to achieve stability across the infinitely varied amount of hardware configurations that customers will want to use their software on.

**Operation System Sprawl**

-   The more operating systems, the harder it is to maintain a consistent environment
    -   Keep it simple
    -   Avoid configuration drift
-   Reasons how new configurations occur
    -   Release versions
    -   Kernel version
    -   Feature packs
    -   Security patches
-   A best practice to reduce the number of versions maintained
    -   Deviation only by exception
    -   Maintained by change management process

In a properly run environment, all operating systems would be properly operationalized. This means that a test and support environment would exist in parallel to the production environment for each version in the organization. All changes to each operating platform would be fully tested in the test environment, and then promoted into production and support environments. 

Configuration drift, occurs when what should be two completely identical servers differ. Drift leads to outages, and unplanned downtime, and should be avoided as much as possible. Reducing the number of operating systems that are present in an environment can serve to exacerbate configuration drift.

## Grid Solutions

-   Grid computing is the combination of computer resources
-   Complete , independent computers are bound together to pool resources
    -   Not administered centrally

-   Similar to massively parallel supercomputers, only bound by IP networks rather than custom connections and interfaces

-   Workloads need to be suited to grid processing
    -   Calculation intensive
    -   Protein folding
    -   Analysis of big data
    -   Trade simulation

Grid computing is the combination of discrete computers are bound together and some of their resources are made available for the processing of jobs from a centralized authority. Each instance of the grid is an independent computer, normally with its own operating system and identity. The grid components have an agent that reports back to a central scheduler to receive jobs and send completed results back to the central scheduler. The members of the grid need not be expensive, specialized systems, instead could be commodity systems with little to no redundancy. In the event that a grid node fails during the process of a workload, the central scheduler will note that the assigned job was not completed and it could be re-assigned to another grid node to complete, without any data loss.

## Cloud Solutions

-   Workload Abstraction
-   Secure multi-tenancy
-   Deployment Models
    -   Public Cloud
    -   Private Cloud
    -   Hybrid Cloud
    -   Hosted Services
-   Examples
    -   Microsoft Azure 
    -   Amazon EC2

Also known as infrastructure as a service, cloud computing is part of the most recent favorable trends in technology these days. From a financial aspect, cloud solutions that are hosted by external providers allow organizations to shift expenditures from capital to operational expenses, which can provide financial benefit to an IT department.

Secure multi-tenancy is the concept of isolating workloads on a common infrastructure, enabling a hosting provider to be able to provide services for two discrete organizations on shared server, network, and storage infrastructure without allowing either organization to view the others data. Shared services will generally cost less for consumers, as the providers are able to spread out the cost of infrastructure and services across multiple vendors. One of the challenges around shared infrastructure is with the issue of compliance, such as the SEC for broker/dealers and HIPPA for healthcare providers that store PHI/Confidential data. 

There are multiple deployment models for cloud services:

-- Public cloud would be cloud services provided by a third party

-- Private cloud refers to clouds that are built internal to an organization for internal consumption

-- Hybrid cloud refers to a mix of public / private cloud solutions and traditional infrastructure

-- Hosted services is different from cloud services, more solution specific like email or CRM

# Resources

**Articles:**

**Blogs / Webcasts / News / Reference Resources:**

**Training:**

**Certifications:**

