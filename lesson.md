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

In brief, server clustering helps provide security against outages that originate from software failure, hardware failure, and outages that happen from unrelated events operating against the physical server site. 


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


## Part 2 - Load Balancer


Load balancing refers to efficiently distributing incoming network traffic across a group of backend servers, also known as a server farm or server pool.

Modern high‑traffic websites must serve hundreds of thousands, if not millions, of concurrent requests from users or clients and return the correct text, images, video, or application data, all in a fast and reliable manner. To cost‑effectively scale to meet these high volumes, modern computing best practice generally requires adding more servers.

A load balancer acts as the “traffic cop” sitting in front of your servers and routing client requests across all servers capable of fulfilling those requests in a manner that maximizes speed and capacity utilization and ensures that no one server is overworked, which could degrade performance. If a single server goes down, the load balancer redirects traffic to the remaining online servers. When a new server is added to the server group, the load balancer automatically starts to send requests to it.

In this manner, a load balancer performs the following functions:

- Distributes client requests or network load efficiently across multiple servers
- Ensures high availability and reliability by sending requests only to servers that are online
- Provides the flexibility to add or subtract servers as demand dictates


![image](https://user-images.githubusercontent.com/106639884/185006473-f9ee5f80-720f-402b-bd10-5710099bc16f.png)


### Benefits of Load Balancing

- Reduced downtime
- Scalable
- Redundancy
- Flexibility
- Efficiency

---

## Part 4 - Blacklisting

![image](https://user-images.githubusercontent.com/106639884/185005618-1811f977-8ebe-44c7-902b-ea754fe48dda.png)


Establishing which entities should be blacklisted is a step in the blacklisting strategy. A blacklist is a list of suspect or hostile entities to which access to a network or system should be forbidden.

A border control authority, as an illustration in the real world, might keep a blacklist of known or suspected terrorists. A store owner might keep track of shoplifters on a blacklist. A blacklist of malware, including viruses, spyware, Trojan horses, worms, and other forms of malware, is common in the area of network security. A blacklist of individuals, IP addresses, programs, emails, domains, processes, or organizations is another option. Blacklisting can be used for almost every part of your network.

By looking at their digital signatures, heuristics, habits, or other characteristics, you can spot suspicious or malevolent entities. Organizations can use lists made by third parties, such as network security service providers, as well as their own blacklists to delist applications. The classic method of access control is blacklisting, which has long been employed by spam filters, intrusion detection systems, anti-virus tools, and other security software applications.

The blacklist approach is threat-centric, and the default is to allow access. Any entity not on the blacklist is granted access, but anything that’s known or expected to be a threat is blocked.

To sum up:

- Blacklisting involves blocking access to suspicious or malicious entities.
- The default is to allow access. 
- Blacklisting is threat-centric.


### Pros and Cons of Blacklisting

One of the biggest pros of the blacklisting approach is its simplicity. It works based on a simple principle — just identify the known and suspected threats, deny them access and let everything else go.

For users, it’s a relatively low maintenance approach. In many cases, your security software or security service provider will handle compiling the list with little need for input from the user.

A blacklist can never be comprehensive, though, since new threats emerge constantly. Every day, the AV-TEST Institute, which researches IT security, registers more than 350,000 new malicious programs and potentially unwanted applications. While keeping up with these threats is challenging, threat information sharing can help make blacklists more effective.

Even with information sharing, it’s easy for security software providers to miss threats simply because there are so many. While blacklisting is effective against known threats, it’s useless against new, unknown threats like zero-day attacks. If your organization is unlucky enough to be the first to be hit with a new kind of attack, blacklisting won’t be able to stop it.

Hackers also sometimes design malware specifically to evade detection by tools that use a blacklist system. They may be able to modify the malware so the blacklist tool does not recognize it as a blacklisted item.


---


## Part 5 - Whitelisting


![image](https://user-images.githubusercontent.com/106639884/185005606-764539fe-40c0-461d-9d84-27600c692613.png)


Whitelisting tackles the same challenges as blacklisting but uses the opposite approach. Instead of creating a list of threats, you create a list of permitted entities and block everything else. It’s based on trust, and the default is to deny anything new unless it’s proven to be acceptable. This results in a much stricter approach to access control. It’s analogous to denying everyone access to your office building unless they can pass a background check and have the credentials to prove that they did.

The whitelisting strategy, for example, is used when a firewall only permits specific IP addresses to enter a network. The Apple app store is another illustration that most people have encountered. The business only allows consumers to use programs that Apple has authorized and added to the app store.

The simplest method for adding programs to a whitelist is to recognize them by their file name, size, and directory path. The issue with this method is that hackers might make a program that has the same file name and size as a whitelisted app, which would allow it to infiltrate the system. You can employ a tougher strategy to avoid this risk, as advised by the National Institute of Standards and Technology (NIST) of the United States. It makes use of digital signatures created by the creator or maker of each component as well as cryptographic hashing techniques.

You must take into account all of the jobs that users must carry out and the tools they'll require to do so in order to develop a whitelist for the network level. In addition to more specific information like application dependencies, software libraries, plugins, extensions, and configuration files, this network-level whitelist may also contain network infrastructure, sites, locations, applications, users, contractors, services, and ports. A user-level whitelist could contain files, applications, and email addresses. You must take into account both user privileges and user activities while using the whitelist strategy.

Organizations can create their own whitelists or work with third parties that typically create reputation-based whitelists and give ratings to software and other items based on their age, digital signatures and other factors.

To sum up:

- Whitelisting involves only allowing access for approved entities.
- The default is to block access.
- Whitelisting is trust-centric.

---

## Part 5 - Activity

Prepare presentation with your own group about which method that will you use to handle these case

Case:

eCommerce
Financial Institution
Government
Personal Static Website
eMail Application


Method:

Clustering
Load Balancing
Whitelisting
Blacklisting
You may combine more than 1 method and give details what and why you do it.
