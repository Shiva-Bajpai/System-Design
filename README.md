# **System Design Learning Playlist 🎯**  

Welcome to the **System Design Learning Playlist**, a curated collection of topics and concepts to help you master system design. Whether you're preparing for interviews or aiming to build scalable systems, this playlist covers the fundamentals, key components, and advanced topics of system design.

---

## **Contents**  
### **1. Basics of System Design**

- 📌 **Scalability:** Scalability refers to the ability of a system to handle increased workload by either adding resources or making better use of existing resources without significant performance degradation.

**Types of Scalability:**
1. Vertical Scaling (Scale-Up): Adding more resources (CPU, RAM, storage) to a single server.
Example: Upgrading from a 4-core CPU to an 8-core CPU on a database server.
Pros: Simple implementation, no changes in architecture.
Cons: Limited by hardware capacity and can become expensive.
2. Horizontal Scaling (Scale-Out): Adding more servers to distribute the load.
Example: Adding more web servers behind a load balancer to handle high traffic.
Pros: Virtually unlimited scalability, redundancy.
Cons: Complex architecture, requires changes in application design.

**Example**
Imagine an e-commerce website like Amazon. During peak sales events (e.g., Black Friday), traffic spikes.
Vertical Scaling: Upgrade the database server to handle more transactions.
Horizontal Scaling: Add multiple application servers to balance the load and ensure smooth user experience.

- 📌 **Reliability:** Reliability is the ability of a system to perform its intended function consistently and correctly, even in the face of failures.

**Strategies for Ensuring Reliability:**
1. Redundancy: Duplicate critical components (e.g., servers, databases) to ensure backup in case of failure.
Example: Two database servers (primary and replica) to ensure no data is lost during a failure.

2. Fault Tolerance: Designing systems to continue functioning even if some components fail.
Example: Netflix uses Chaos Engineering to test system reliability by deliberately causing failures.

3. Data Backups: Regularly backup critical data to ensure recovery in case of disaster.
Example: A bank might back up transaction logs every hour.

**Example:**
Online Banking System: Users expect uninterrupted service even if one of the servers goes down. Redundancy ensures backup systems take over seamlessly.


- 📌 Availability  
- 📌 Latency and Throughput  
- 📌 CAP Theorem  

### **2. Networking Concepts**
- 📌 Load Balancer  
- 📌 CDN (Content Delivery Network)  
- 📌 DNS (Domain Name System)  
- 📌 Reverse Proxy  
- 📌 Firewall  

### **3. Databases**
- 📌 SQL vs NoSQL  
- 📌 Database Sharding  
- 📌 Replication and Consistency  
- 📌 Indexing  
- 📌 Transactions (ACID Properties)  

### **4. Caching**
- 📌 Cache Basics  
- 📌 Cache Eviction Policies (LRU, LFU)  
- 📌 Distributed Caching (Redis, Memcached)  
- 📌 Write-Through vs Write-Back Cache  

### **5. APIs and Communication**
- 📌 REST APIs  
- 📌 GraphQL  
- 📌 WebSockets  
- 📌 RPC (Remote Procedure Call)  
- 📌 Message Queues (Kafka, RabbitMQ)  

### **6. Scalability and Performance**
- 📌 Horizontal vs Vertical Scaling  
- 📌 Database Partitioning  
- 📌 Distributed Systems (MapReduce, Hadoop)  
- 📌 Rate Limiting  
- 📌 Circuit Breakers  

### **7. Monitoring and Logging**
- 📌 Application Monitoring (Prometheus, Grafana)  
- 📌 Centralized Logging (ELK Stack)  
- 📌 Alerting and Incident Response  

### **8. Design Patterns**
- 📌 Microservices Architecture  
- 📌 Monolithic vs Microservices  
- 📌 Event-Driven Architecture  
- 📌 CQRS (Command Query Responsibility Segregation)  
- 📌 Saga Pattern  

---

## **How to Use This Playlist**  
1. **Start with the Basics:** Build a strong foundation by understanding the core principles of system design.  
2. **Learn Component-Wise:** Focus on one category at a time, such as databases, networking, or caching.  
3. **Practice:** Use real-world scenarios to design systems like social media platforms, e-commerce websites, or chat applications.  
4. **Iterate and Review:** Revisit concepts as needed and continuously refine your understanding.  

---

## **Goals of This Playlist**  
- 🌟 Gain a practical understanding of system design concepts.  
- 🌟 Learn how to handle scalability, performance, and reliability challenges.  
- 🌟 Prepare for system design interviews with confidence.  

---

**Happy Learning! 🚀**  
Let’s design systems that scale! If you have any suggestions or want to contribute, feel free to reach out.  
