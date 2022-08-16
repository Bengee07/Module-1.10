## Brief

### Preparation

Write about any preparations needed for the lesson, such as tools, installations, prior-knowledge, etcs.

### Lesson Overview

Write about how instructors can brief the students at the start of the lesson. It is good to guide students through what is going to be covered and the outcome. Setting expectations.

---

## Part 1 - Server Clustering

When several servers collaborate on a single system to give users improved availability, this is referred to as server clustering. By allowing a different server to take over in the event of an outage, these clusters are utilized to minimize downtime and outages. This is how it goes. One system is linked to a number of servers.

Before the client feels any downtime, the workload is shifted to another server the instant one of these servers encounters a service interruption. File, print, database, and message servers are the most often used clusters, and they are typically utilized for applications with regularly updated data. In general, clustering servers provide customers with a higher level of availability, dependability, and scalability than any single server is capable of providing.

Each server in a clustered server environment is in charge of owning and managing each of its own devices, as well as having a copy of the operating system and any programs or services that are used to run the other servers in the cluster. The computers in the cluster are configured to cooperate in order to improve data security and sustain the cluster configuration over time.


The main justification for server clusters is uptime and outage prevention. Clustered servers, as previously discussed, provide improved security against a network falling offline due to a power outage. Servers in a cluster are guarded against three different kinds of outages.

In brief, server clustering helps provide security against outages that originate from software failure, hardware failure, and outages that happen from unrelated events operating against the physical server site. We'll go into more depth about these sorts of failures in the next sections.


**Application / Service Failure**

Any disruptions that result from serious mistakes with software or services that are essential to the server's or data center's functioning are referred to as application/service failure events. Numerous circumstances, many of which are largely inescapable, can contribute to these failures. Application/service failures are by their very nature challenging to predict and prepare for, even though most servers incorporate redundancy mechanisms to prevent this form of failure.

It can be challenging for server administrators to identify and fix possible problems before they result in an outage due to the complicated and dense nature of server monitoring data. While a watchful, competent, and proactive server administrator can spot these problems and deal with them before they become serious ones, no server administrator will be able to offer complete protection from this kind of failure.


**System / Hardware Failure**

Failures with the actual hardware that the server is running on are the cause of this kind of outage. These outages can be brought on by a wide range of variables and can affect practically every sort of component essential to the operation of a server or data center.

Although the functionality and dependability of server components are always increasing, no component is impervious to failure. Overheating, inadequate optimization, or just the component reaching the end of its useful life are all potential causes of this failure. Due to their significance in ensuring the server's continued operation, processors, physical memory, and hard disks are among the components most prone to failure.

**Site Failure**

Site failures are typically brought on by incidents that take place outside of a data center. Although there are numerous events that could theoretically result in a site failure, those that do so most frequently are natural disasters that result in widespread power outages and those that have the potential to harm the data center's hardware.

While some consequences of natural disasters cannot be eliminated by anything other than a careful selection of locations, those brought on by power outages and the issues they bring can be anticipated by adopting redundancy techniques like server clusters. These redundancy solutions are essential for data centers situated in disaster-prone areas.

Even while problems that can cause these three different kinds of failures can be found and fixed, redundancy techniques like server clustering are the only way to guarantee almost perfect reliability. Server clustering is a fantastic approach to ensure that data centers always operate at peak performance levels throughout the year.


---


## Part 2 - The Three Types of Clustering Servers

Based on how the cluster system (also known as a node) is connected to the device responsible for storing configuration data, there are three different types of server clusters. The three varieties are discussed in more detail below and comprise a single (or standard) quorum cluster, a majority node set cluster, and a single node cluster.


1. Single (or Standard) Quorum Cluster

This cluster, which is the most widely used, consists of several nodes and one or more cluster disk arrays that use a single connection device (called a bus). Each of the various cluster disk arrays in the cluster is managed and owned by a single server. The mechanism utilized to establish whether or not each specific cluster is up and secure is referred to as the titular quorum.

In practice, single quorum clusters are rather straightforward. Every node has a "vote" that it uses to let the central bus know that it is online and working. A single quorum cluster will continue to function as long as more than 50% of its nodes are online. The cluster won't continue to operate until the problems with the individual nodes are resolved if more than 50% of the nodes in it are unresponsive.


2. Majority Node Set Cluster 

This cluster is similar to the one mentioned before, but it varies in that each node has a copy of the configuration data for the cluster, and that copy is identical on every node. The clusters with individual servers spread across multiple regions will benefit the most from using this architecture.

While majority node set clusters and single quorum clusters both function similarly, the former differs in that it doesn't require a shared storage bus to work because each node holds a copy of the quorum data locally. The benefit of a common bus isn't fully eliminated by this, but it does give configuration options for remote servers more leeway.

3. Single Node Cluster

This model has a single node and is most frequently used for testing purposes. Although single node clusters are frequently employed in the creation and study of cluster systems, their usefulness is severely constrained by the absence of failover. All cluster groups become unavailable when a single node fails because they are made up of only one node.

A customer service agent at a nearby data center or web hosting company may go over the differences between the three models in further depth and help you choose the one that will work best for your company. In general, the Standard Quorum Cluster is your best option unless you have unusual demands (or are located in several, geographically scattered sites).

---

## Part 3 - Server Environments Differentiation

The utilization of numerous environments is a suggested procedure for any big software development project, regardless of how your DevOps process appears and the many tools you employ. Before being deployed and made accessible to consumers, your product will have undergone thorough testing thanks to the utilization of numerous environments.

You should have minimum of two types of server environments: the Local Test Server and Production Server(s).


**Development**: The development environment would be the first line of defense against bugs. Here, developers deploy their code and test any newly implemented features. Any bugs found are dealt with before re-deploying for further testing. The process is iterated until the code is ready for the next stage of testing.


**Staging**: Once developers are satisfied with their code and consider it fairly stable, it is then deployed to the staging environment for further testing. This is where Quality Assurance (QA) is performed. Testers access the staging servers and ensure that the application works as it should. They run test cases to detect bugs and run performance tests to find areas that could be improved. Any bugs or enhancements are reported back to the developers and the process is repeated until the code passes the staging phase.


**Production**: Once the code has been thoroughly tested, it is then pushed to production where it is made available to end-users.


The three typical environments for software projects are shown in the environment configuration above, which is merely an illustration. Depending on the requirements of your team and project, your setup may change. You could set up more or fewer environments; for example, some prefer to have a Pre-production environment to test the code more thoroughly before the final deployment to Production, while others keep separate Staging and QA environments, where developers run additional tests (such as integration tests) in the Staging environment and the QA environment is used only for quality assurance testing.

---

## Part 4 - Insert Summary

Insert Instructions
