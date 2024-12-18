##          Load  BALANCING
Load balancing is the distribution of inbound network traffic among several backend servers, commonly called a server farm or pool. Modern high-traffic sites have to handle several thousand, if not tens of millions, of concurrent requests from users or clients and quickly provide the right content, pictures, videos, or application data. To scale to such enormous numbers cost-effectively, current best practices in computation usually necessitate adding more servers.
### What Is a Load Balancer?
A load balancer is a hardware or software tool that acts as a reverse proxy to distribute incoming traffic across the available servers in a server farm (following static or dynamic algorithms) so that traffic is routed optimally and applications can perform correctly.

A load balancer functions as a wall at the forefront of the servers, distributing client demands across all servers that can fulfill them. It does this in a way that maximizes speed and capacity utilization while guaranteeing no server is overwhelmed, something that can negatively impact performance.

If a single server becomes unavailable, the load balancer reroutes traffic flow to the online residual servers. When an additional server gets included in the group, the load balancer sends requests to it automatically. This makes load balancers critical to any network, data center, mainframe, or server infrastructure.

#### Types of load balancers
While the main purpose of a load balancer may seem simple, its underlying operations are extremely sophisticated, allowing it to power high-volume and complex networks. Various types of load balancers have emerged to fulfill different network technology needs, such as:

1. **Hardware load balancers:** A hardware-led load balancer is a hardware tool that can safely process and reroute gigabytes of traffic among hundreds of different servers. You can house it in your data center and construct numerous virtual load balancers employing virtualization, or you can even operate it manually.

2. **Software load balancers:** Software-based load balancers are apps that conduct all the functions of load balancing. They are available for installation on any server or through a managed third-party service. Some network systems may have software-based load-balancing functions built in.

3. **Global load balancers:** These load balancers can function across various geographically dispersed servers. Companies can, for instance, possess servers in multiple data centers in different countries and on the cloud managed by third parties. Local load balancers handle the application burden within a specific area or zone in this situation. They shift traffic to a local server to reduce latency. However, in the event of server failure, they may need to reroute traffic to sites or servers in a different region, and this is where global load balancers come into play.

4. **Application balancers:**
Multiple server farms with an assortment of servers devoted to a particular application are present in modern applications. To divert traffic, application load balancers analyze the request’s content. Consider an ecommerce application; the application load balancer forwards queries to view products to servers, which include images and videos but do not require active connections. It sends requests from purchasing carts to servers that can sustain multiple connections and store cart details for a longer duration.

5. **Network balancers:** Network load balancers analyze internet protocol (IP) addresses along with additional network data to optimally move traffic. They can track the origin of application traffic and allocate static IP numbers to multiple servers. Network load balancers manage server demand via static and dynamic load balancing algorithms

#### some techniques for traffic load balancing:
* Weighted Round Robin
Similar to Round Robin, but it distributes network load based on each server's capacity. This is useful when diverting requests across servers with different capabilities. 
* Round Robin
Distributes DNS name resolution requests in a circular pattern among virtual servers. Over time, each server receives an equal number of connections. 
* Weighted load balancing
Assigns more connections to specific nodes based on their weight value in the configuration. This is useful when back-end nodes have different hardware or some nodes receive more traffic. 
* Dynamic load balancing
Adjusts the distribution of network traffic in real-time based on the current state of the network or servers. Dynamic load balancers monitor server performance and health. 
* Global server load balancing (GSLB)
Distributes traffic across geographically dispersed servers. This is useful for web applications with a global user base. 
* Least connection load balancing
Helps control the load on application instances more fairly when some requests take longer to complete. 
* Session persistence
Also known as Sticky Session, this algorithm directs all requests from a user session to the same server. This is useful for applications that need to maintain session information, such as e-commerce shopping carts. 

When choosing a load balancing technique, one can consider things like the nature of the workload, server capacity, application requirements, and budget constraints. 