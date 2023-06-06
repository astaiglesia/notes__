# System Design

> SDI Preparation
*sdi prep focuses on 2 crucial aspects*
- gain a deep understanding of fundamental system design concepts
- study and practice answering common sdi questions

> goals of an SDI: 

- demonstrate ability to design and implement a scalable system that can handle a ton of traffic, data, and users
- demonstrate problem-solving skills
- show how you make design decisions
- demonstrate effective communication



## resources:

[2023 SDI Survival Guide](https://levelup.gitconnected.com/system-design-interview-survival-guide-2023-preparation-strategies-and-practical-tips-ba9314e6b9e3)


[Coding Interview University](https://github.com/jwasham/coding-interview-university)


[system design primer](https://github.com/donnemartin/system-design-primer)

[desigining data-intensive applications](hardcopy) : min: [ch3, ch5, ch6]

[grokking sys design fundamentals](https://www.designgurus.io/course/grokking-system-design-fundamentals) : use free material alongside concept search
[grokking sys design interview](https://www.designgurus.io/course/grokking-the-system-design-interview) : use free material alongside concept search

[cracking the coding interview](hardcopy) : check for relevent info

[10 common sdi questions](https://levelup.gitconnected.com/10-system-design-interview-questions-with-answers-i-wished-i-knew-before-the-interview-31dcfc3cddef)


[7 must read research papers](https://www.designgurus.io/blog/sys-design-papers)



<br>
<hr>

## study path
<hr>

re-learn fundamentals > do a few problems > design patterns block > do more problems

[] review fundamental system design concepts
[] select 5 init sdi questions
  [] complete 1st sdi-q

[] migrate/aggregate extg system design notes (algo-expert notes are in one note)
  [] complete 2nd sdi-q

[] deep dive design patterns
  [] complete 3rd sdi-q

[] refine terms and concepts with chat gpt reponses
  [] refactor defs to actual sdi responses
  [] complete 4th sdi-q

[] [what distinguishes candidates in an sdi](https://interviewnoodle.com/system-design-interviews-what-distinguishes-you-from-others-7095405ec48)
  [] complete 5th sdi-q
  [] select next sdi-q's


<br>


## fundamentals of system design
<hr>

* **be able to apply knowledge to real world scenarios**
* **understand concept application to different types of systems** => explain our designs' balance, tradeoffs and desirable system characteristics
* **be able to balance business requirements with the constraints and limitations of our designs**
<br>


### terms & concepts
 [18 system design concepts every engineer should know](https://www.designgurus.io/blog/system-design-interview-fundamentals)

> [] **Availability**

> [] **ACID Properties**

> [] **API Gateway**

> **Caching**
> - storing of frequently accessed data in a high speed storage layer
> - reduces the load on the underlying data store
> - improves system performance 

> [] **CAP Theorem**

> [] **CDN**

> [] **Checksum**

> [] **Consistency**

> [] **Databases**
      [] replication
      [] SQL / Relational
      [] Non-Relational / NoSQL
      [] indexing

> [] **Data Partitioning**
      [] horizontal / sharding
      [] vertical

> [] **Distributed Coordination Services**

> [] **Distributed File Systems**

> [] **Distributed Messaging Systems**

> [] **Domain Name System (DNS)**

> [] **Fault Tolerance** 
> - the ability of a system to continue functioning despite component(s) failure(s)
> - redundancy and load balancing can increase a system's fault tolerance

> [] **Full Text Search**

> [] **Heartbeat**

> [] **Latency**

> [] **Load Balancing / Balancer**
> - the optimization of resource usage and server loads by distributing workloads across multiple machines to prevent overloads

> [] **Microservices**

> [] **Notification System**

> [] **Partial Tolerance**

> [] **Partitioning**

> [] **Proxies**
      [] Forward
      [] Reverse


> **Scalability** : the ability of a system to handle increased load / traffic
> - **horizontal scaling** : increasing hardware to support addtl traffic (more machines)
> - **vertical scaling** : increasing hardware resources to a single machine (bigger machine)


> [] **SQL vs NoSQL**

> [] **Throughput**



    [] real-world use cases : examine scenarios && applications



<br>

## common design patterns
> [] **microservices**
> [] **event sourcing**
> [] **sharding**
> [] **cqrs**
> [] **reverse proxy**
> [] **circuit breaker**
> [] **backpressure**
> [] **object pool**



## databases
> [] **relational**
> [] **non-relational / nosql**
> [] **document db**
> [] **distributed key-value stores**
> [] **graph db**
> [] **time-series db**



## distributed systems and algorithms
> [] **merkle tree**
> [] **consistent hashing**
> [] **read repair**
> [] **gossip protocol**
> [] **bloom filter**
> [] **heartbeat**
> [] **CAP and PACELC theorems**


## SDI Problems

### how to answer an sdi-q
[the 7 step process](https://www.designgurus.io/blog/complete-guide-sys-design)
[time mgmt in the sdi](https://www.designgurus.io/blog/step-by-step-guide)
> **requirement clarification** : find and define the scope
> **back of the envelope estimation** : estimate the scale of the system
> **system interface definition** : define the necessary api's expected of the system
> **define the data model** : define the tables and layout
> **high level design** : describe the core components of the design system
> **detailed design** : dig deeper into 2 or 3 major components
> **identify and resolve bottlenecks** : discuss friction points and possible solutions

[**--> the system design master template <--**](https://levelup.gitconnected.com/system-design-master-template-how-to-answer-any-system-design-interview-question-ee5dc332acd5)

## Interview Tips
- utilize a similar approach to algo solving
- demonstrate your ability to anticipate and address potential issues in the design
  - acknowledging and addressing negative aspects and potential issues builds trust and credibility with the interviewer


> **COMMUNICATE YOUR THOUGHT PROCESS**
think out loud & talk through the problem <algotraining_skills!>
  
  - *restate the problem* 
    - note the system requirements and constraints
    - note initial points of consideration 
    - note possible approaches and tradeoffs
  - *break down the problem*
  - *use diagrams and sketches*
  - *discuss tradeoffs and constraints*
  - *provide support to your design choices*
  - *be prepared to answer questions on your design and provide alternatives*
  - *be open to feedback*



> **WHAT ARE THE EDGE CASES??**
  - *anticipate edges*
  - *plan for failure*
  - *consider scalability*
  - *consider security*
  - *explain your reasoning*

### [top system design interview questions](https://levelup.gitconnected.com/10-system-design-interview-questions-with-answers-i-wished-i-knew-before-the-interview-31dcfc3cddef)

[more q.s](https://medium.com/geekculture/top-12-system-design-interview-questions-with-answers-2022-dc2b6599f39a)

Design: 
> Facebook Messenger
> Youtube
> Facebook’s Newsfeed
> an API Rate Limiter
> Twitter
> Dropbox or Google Drive
> a Web Crawler
> Twitter Search
> a URL Shortening service like TinyURL
> Instagram
> Yelp or Nearby Friends
> Ticketmaster

## notes
<hr>

> SDI Survival Guide


