---
title: "Common Application Services"
keywords: 
sidebar: mydoc_sidebar
toc: true
permalink: cas.html
folder: competency_model
summary: "Directory services provide a number of benefits, mapping names to resources."
tags:
  - infrastructure_architecture
---

# Description 

Infrastructure applications are those that provide infrastructure services, which can be consumed by servers and business applications alike. Every environment has these components in some form or another, whether they are automated or not.

# Overview

## Directory Services

Directory services provide a number of benefits, mapping names to resources. For example, DNS maps names to computers, and Lightweight Directory Access Protocol (LDAP) maps usernames to directory objects/security context. Most of directory services fall into the realm of authentication, authorization, and accounting services (AAA). Authentication is the mechanism by which systems identify their users, authorization is the mechanism by which access permissions are determined for a particular user (security context), and accounting is the tracking of network resource consumption.

For example, if a user wants to get data from a file share, they go through the AAA process to achieve this in a secure environment. First, they will authenticate themselves (user security context) against an authority that has control over the resource that they want to access, namely the file share. Once authenticated, the access control lists (ACLs) on the share, directory, and file will be compared against the permissions to see if the desired action can be accomplished under the user's provided security context, which would be authorization. Finally, a record of the authentication and activity will be logged, which is account and providing the final A of the AAA.

Identity comes in a lot of flavours, but the most common model these days is that of a class/object/attribute model, which we will discuss later. Directory services provide a location to store all these forms of identity, such as user, group, and computer objects. The most common directory type is of the LDAP variety, such as Oracle Internet Directory, Red Hat Enterprise Directory, or Active Directory. LDAP is a descendent of X.500, leaning it out and making it easier to implement, hence the "lightweight" portion of the name.

Should someone in the class note that Active Directory is not LDAP, attempt to reach middle ground and don't press the point, as this is common fodder for killing hours with debate that will amount to little. Sort of like the wars that occur over PC vs. Mac, or Emacs vs. VI.

## Identity and Access Management

Identity paradigm refers to a single entity, which can map to multiple identities, which of which map to unique attributes. For example, I am a single person with three email accounts (gmail, hotmail, and yahoo), and each services have a different username and password. This is the challenge that IaM attempts to resolve, by unifying identity either into a centralized location or by synchronizing identity across multiple discrete repositories. In most environments, a single entity would be designated the authoritative source of identity for an organization. Most commonly, this is provided by the systems for human resources (HR) which track all the full time employees, contractors, and vendors within an organization.

Single sign-on and same sign-on are two different methods for implementing identity management, from an end user perspective. The key difference between the two is that single sign-on occurs once and assigns a token or ticket that provides security context, and then all subsequent interactions with other systems occur with that token or ticket. For example, when a user logs into a Microsoft Windows desktop within an Active Directory domain, the user receives a Kerberos ticket that will be used to authenticate to any network resources that are requested and are within the realm of that Active Directory domain, without the user receiving a request for their credentials. Same sign-on is a little different, where the same username and password are used in disconnected directories that are synchronized to ensure that passwords are the same. When a network service is requested, the user enters the same username and password for all services. Most IaM solutions will use a combination of both single and same sign-on due to applications being designed to consume different forms of identity.

Consumption of identity can come through a variety of ways, including the Windows Domain structure or Security Assertion Markup Language (SAML). SAML is one of the open standards that is used for exchanging authentication and authorization information. SAML has three distinct participants: Service Provider, User Agent, and Identity Provider. The service provider would be the application that is being accessed, user agent being the method of access (for web base applications, it would be a web browser), and the identity provider who can authenticate the assertion that was made.

Directory services, as noted before, are the repository for identity. Token services facilitate brokered authentication, providing a method to allow users to authenticate themselves to a resource without having to go through a full authentication cycle every time. Authentication itself is a weighty process, thus required methods to streamline things to provide better scalability. Token services include Web Service -- Security (WS-Security) process, which is an open source initiative and can be found in detail on the web. Essentially, once an authentication has occurred, a security token is issued, which is then presented when access to resources are desired. The resource receives the token, validates it against the authority, and then provides access.


Federation services are similar to token services, but span pools of identity. One organization will provide federation to a second organization, trusting the second organization to authenticate their users appropriately. Resources can be shared without the overhead of having to share significant quantities of information between one another. At a high level, federation works by creating a role within an organization that maps to users coming from a second organization, providing a local security context. The best example of federation is around calendar information within a messaging environment, where two organizations will allow calendar data to be shared to facilitate communication and meetings and what not. A user authenticates in their home organization, and  makes a security assertion to the second organization, who verified that the assertion is valid and then provide the requested data.

## Network Services

Network and naming services are those that help us find resources in an environment. DNS and WINS are used to map node names to addresses, with the latter being almost exclusively used by Windows networks and is rapidly being deprecated in many organizations.

Dynamic Host Configuration Protocol (DHCP) is a network service that provides critical networking information to clients on request, including IP addresses. This allows a system to come up on a network, ask for an IP address, and be provided one that is already not in use along with other information like gateway, netmask, dns servers, etc.

Quality of Service, or QoS, is a method of setting preference for traffic across a network. Switches, routers, and firewalls will show a preference for traffic on a specific port or traveling to/from a specific location. This is important for things that are time sensitive, like voice over IP communications.

## Domain Name Services


Domain Name Service (DNS) is used to convert IP addresses and short names into fully qualified domain names (FQDN) that can be used to address other networked hosts.

DNS is a critical network service that facilitates communication between nodes within a network by name, rather than by IP address. In the previous slide, the resolution of the host name to IP came from within the system itself via a hosts file. If the hosts file did not contain the required entry, DNS could be used to determine the address of the host.

DNS works in a hierarchy, with the top level domain (TLD) providing authoritative information about the subdomains that are contained beneath it. This recursion continues until an authoritative response is received regarding the request, normally an "A" record request for a host.domain. For example, if we wanted to look up www.dot.state.tx.us, we would first query the root top level domains to be directed to a name server that would have authority over the .us domain. This name server would then be queried regarding .tx.us., which would point us to another name server that would be authoritative for .tx.us. and then to ask about .state.tx.us, and so forth. During the above example, we refer to multiple name servers, but this is not always the case. A single name server can be partitioned and authoritative for a hierarchy, but would handle each query as though it was redirecting to a new name server. Assuming that www.dot.state.tx.us was handled by a single name server that had authority over the full hierarchy, it would provide redirection to itself to answer name queries.

**Common DNS record types:**

A -- Address record

CNAME -- Canonical name record, can be thought of as an alias

MX -- Mail exchange

NS -- Name server record

PTR -- Pointer record, can be thought of as a reverse

SPF -- Used for Sender-Policy Framework (SPF), mail relay validation

## Database Services

A database is an organized collection of data, which can be used for one or more purposes by one or more entities. Database theory is a huge topic, such that the author had three classes on it and it alone during college. Databases are commonly intertwined with data theory, which is the domain of the information architect and out of scope for our discussion here. We are not going to dive into the nitty gritty database architect / administrator stuff, either. Instead, we are going to go over databases at a high concept level and then talk about infrastructure and operational architecture considerations.

Databases are managed by a database management system (DBMS), or sometimes relational DBMS (RDBMS), such as Oracle, MySQL, MS-SQL, and many others. Despite this, there are components that provide functionality that is similar to one another.

Interface -- the method by which data is inserted and retrieved, as well as management for the database as well

Query language -- a standard language that is used to do data manipulation. Most common is the structured query language (SQL).

Query engine -- the component that receives the query from the interface and parses it for consumption

Database -- the component that manages the data files, both at the low level on the storage, as well as the structure of the database itself

Transaction -- a transaction is made up of one or more queries, which need to be executed in order and aligned with the ACID process. The transaction engine is charged with the responsibility of ensuring that ACID compliance is maintained through ordering and sequencing the transaction.

Relational in a database context, refers to the idea that data contained within a database is relative to one another. Thus, a table may have multiple attributes, which are keyed off a single attribute using indexes and keys (primary, foreign). For example, address and telephone number are keyed off of user name, making it easier to locate associated data. Not all databases are relational with a key and index system, instead using internal constructs within the software application that uses the database to maintain relationality.

