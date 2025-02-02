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

---***---

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

---**---

- 📌 **Availability:** Availability is the percentage of time a system remains operational and accessible to users.

**Formula:**
Availability (%) = Uptime / Uptime + Downtime × 100 

**Strategies for High Availability:**
1. Load Balancers: Distribute traffic among servers to ensure no single server becomes a bottleneck.
Example: AWS Elastic Load Balancer ensures traffic is spread across multiple servers.
Failover Mechanism:

2. Automatically switch to a backup system if the primary system fails.
Example: A backup server takes over if the main server crashes.

3. Replication: Maintain multiple copies of data or services in different regions.
Example: Cloudflare’s distributed servers ensure website availability even during regional outages.

**Example:**
Video Streaming Platform: Users expect uninterrupted video playback. A failover mechanism ensures smooth streaming if one server goes down.

---**---

- 📌 **Latency and Throughput:**
  
- **Latency** is the time delay between a user’s action (request) and the system’s response. It is typically measured in milliseconds (ms).
**Types of Latency:**
1. Network Latency: Time taken for data to travel between client and server.
Example: Latency increases when streaming a video from a server located in another continent.

2. Processing Latency: Time taken by the server to process the request.
Example: A complex database query might take several seconds to execute.

3. Disk Latency: Time taken to read or write data to storage.
Example: SSDs have lower latency compared to traditional HDDs.
Strategies to Reduce Latency:

4. Content Delivery Networks (CDNs): Store copies of static assets (images, videos) closer to users.
Example: Akamai or Cloudflare reduces video streaming latency by caching content near users.

5. Caching: Store frequently accessed data in-memory for quicker access.
Example: Use Redis to cache user session data.

6. Efficient Algorithms: Optimize code to reduce processing time.
Example: Use binary search instead of linear search for faster data retrieval.

**Example:**
Gaming Application: Low latency is critical for real-time multiplayer games. Players in different countries are connected via geographically distributed servers to minimize latency.

### Throughput
**Throughput:** Throughput is the rate at which a system processes data or requests per unit time. It is usually measured in requests per second (RPS) or transactions per second (TPS).


● **Key Factors Affecting Throughput:**
1. Hardware Capacity: CPU, memory, and disk speed influence the system’s ability to process data.
Example: High-throughput systems often use SSDs and multi-core processors.

2. Concurrency: Ability of the system to handle multiple requests simultaneously.
Example: Thread pools in Java allow concurrent processing of tasks.

3. Bottlenecks: Any component (e.g., database) that limits the overall system throughput.
Example: A slow database query can reduce the throughput of a web application.


● **Strategies to Improve Throughput:**
1. Horizontal Scaling: Add more servers to distribute the load.
Example: Distribute database queries across multiple replicas.

2. Batch Processing: Group multiple requests and process them together.
Example: Payment gateways process transactions in batches during peak hours.

3. Queue Management: Use message queues (e.g., Kafka, RabbitMQ) to handle high traffic.
Example: An e-commerce platform uses a queue to process millions of order requests during flash sales.

**Example:**
Payment Processing System: A payment gateway like PayPal needs to process thousands of transactions per second. Using distributed servers and message queues ensures high throughput.

___**___

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
