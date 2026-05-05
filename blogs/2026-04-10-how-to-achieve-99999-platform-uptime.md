---
title: "How to achieve 99.999% platform uptime"
url: "https://tyk.io/blog/how-to-achieve-99-999-platform-uptime/"
date: "Fri, 10 Apr 2026 13:28:58 +0000"
author: "Laura Heritage"
feed_url: "https://tyk.io/feed/"
---
<p><span style="font-weight: 400;">Need to build a highly available, ultra resilient financial platform? In a world of shifting customer loyalties and ever-new attack vectors, doing so is crucial to financial institutions’ long-term success. </span></p>
<p><span style="font-weight: 400;">At the LEAP 2026 conference, Arunkumar Ganesan, a distinguished engineer at CapitalOne, shared his experience of building financial platforms for 99.999% (“five nine”) uptime. </span></p>
<p><span style="font-weight: 400;">Prior to 2019, CapitalOne had multiple lines of business creating duplicate solutions and capabilities, fragmented tools, and different standardizations for resiliencies and availability, resulting in lots of incidents and availability concerns. Its solution was to build foundational platforms with common capabilities to encourage reuse, provide standardization, and support innovation at scale. </span></p>
<p><span style="font-weight: 400;">You can </span><a href="https://youtu.be/0_RXpf1Dqqo?si=hV5GQgQAHHyhb6c5"><span style="font-weight: 400;">watch Arunkumar’s full explanation of how CapitalOne achieved it</span></a><span style="font-weight: 400;"> or read on for the top takeaways. </span></p>
<h2><span style="font-weight: 400;">Focus on resilience and reliability </span></h2>
<p><span style="font-weight: 400;">Building standardized platforms for 14,000+ users requires those platforms to be highly resilient, available, and user-friendly. That means focusing on both architectural patterns and non-architectural concerns. </span></p>
<p><img alt="" class="alignnone wp-image-7655 size-large" height="447" src="https://tyk.io/wp-content/uploads/2026/04/blog-achieve-99percent-uptime-1-1024x572.png" width="800" /></p>
<h2><span style="font-weight: 400;">Architecture </span></h2>
<p><span style="font-weight: 400;">Architecture is the backbone of achieving high availability. With the right architecture, you can eliminate single points of failure in your deployment:</span></p>
<ul>
<li style="font-weight: 400;"><span style="font-weight: 400;">In the cloud, you can do so using two regions with multi-availability zones for auto-replication and auto-scaling. </span></li>
<li style="font-weight: 400;"><span style="font-weight: 400;">To support microservice availability, you can build microservices into a particular business domain or business capability, avoiding tightly coupled service dependencies. </span></li>
<li style="font-weight: 400;"><span style="font-weight: 400;">For platforms that require both batch and real-time users, separate them out with a cluster specifically for batch processing and another for real-time users, with different resiliency patterns (to avoid batch-related spiky loads impacting users). </span></li>
<li style="font-weight: 400;"><span style="font-weight: 400;">Bake redundancy in by separating databases from real-time user traffic for high reliability. </span></li>
</ul>
<h2><span style="font-weight: 400;">Mandatory resiliency standards</span></h2>
<p><span style="font-weight: 400;">If high availability and resiliency are your targets, you’ll need to define some goals. CapitalOne did this by grouping goals into three areas:</span></p>
<ol>
<li><span style="font-weight: 400;"> Deployment and scalability: </span></li>
</ol>
<ul>
<li style="font-weight: 400;"><span style="font-weight: 400;">Geographic distribution: Must deploy across at least two distinct geographical regions. </span></li>
<li style="font-weight: 400;"><span style="font-weight: 400;">Regional capacity: Each region must independently support 100% of the production workload. </span></li>
</ul>
<ol start="2">
<li><span style="font-weight: 400;"> Architecture and dependencies: </span></li>
</ol>
<ul>
<li style="font-weight: 400;"><span style="font-weight: 400;">Regional autonomy: Cross-region dependencies are strictly prohibited; maintain regional affinity. </span></li>
<li style="font-weight: 400;"><span style="font-weight: 400;">Critical dependency compliance: All critical system dependencies must meet these resiliency standards.</span></li>
<li style="font-weight: 400;"><span style="font-weight: 400;">Data consistency: Data synchronization must be automated and consistently replicated across all regions. </span></li>
</ul>
<ol start="3">
<li><span style="font-weight: 400;"> Failure management and recovery: </span></li>
</ol>
<ul>
<li style="font-weight: 400;"><span style="font-weight: 400;">Service continuity: A single-region failure must not cause a service outage. </span></li>
<li style="font-weight: 400;"><span style="font-weight: 400;">Automated failover: Failover and failback processes must be fully automated. </span></li>
<li style="font-weight: 400;"><span style="font-weight: 400;">Time-based objectives: Strict recovery time objective (RTO) and recovery point objective (RPO) goals. For example, when a service is degraded, it has to be back up within 15 minutes, and when there’s a data problem you should be able to go back at least 15 minutes to the data. </span></li>
</ul>
<p><span style="font-weight: 400;">All CapitalOne platforms must follow these standards. Writing them down clearly for your own organization means that all teams can see at a glance what they must comply with. </span></p>
<p><span style="font-weight: 400;">CapitalOne also uses domain-driven design (DDD), which delivers multiple benefits for platform architecture, including modularity, bounded context services, and scalability. This empowers CapitalOne to set different service level agreements for different capabilities, as well as providing its customers with high flexibility in the way they integrate with specific subdomain services.</span></p>
<p><img alt="" class="alignnone wp-image-7656 size-large" height="435" src="https://tyk.io/wp-content/uploads/2026/04/blog-achieve-99percent-uptime-2-1024x557.png" width="800" /></p>
<h2><span style="font-weight: 400;">Achieving 99.999% availability </span></h2>
<p><span style="font-weight: 400;">Achieving 99.999% availability isn’t simple. It requires a careful balance between understanding your platform’s capabilities and engineering marvels. You need to focus on where you need to apply effort in terms of each capability and what your users need, to know where you need to achieve five nine availability. </span></p>
<p><span style="font-weight: 400;">At CapitalOne, for instance, five nine availability is more critical for transaction processing than for reporting. It’s the same for every organization: Not every single service is critical for your domain. </span></p>
<p><span style="font-weight: 400;">Implementing the standards above (the two-region deployment model with multiple availability zones, and so on), gives you your minimum requirement when it comes to deployments. The diagram below outlines CapitalOne’s minimum requirement model for bounded context service with top tier resilience: </span></p>
<p><img alt="" class="alignnone wp-image-7657 size-large" height="455" src="https://tyk.io/wp-content/uploads/2026/04/blog-achieve-99percent-uptime-3-1024x582.png" width="800" /></p>
<p><span style="font-weight: 400;">On top of this, you’ll need to account for poison pill requests. These requests that kill your services when you process them, such as a customer query that over-fetches and hogs database resources. Poison pill requests can be entirely legitimate but still cause high CPU, high memory, retraced ROMS, and the like.  </span></p>
<p><span style="font-weight: 400;">To avoid such requests bringing your services down one by one, you can build customer traffic-based circuit breakers. These can identify poison pill requests and stop the system accepting any further requests to reduce the blast radius to that particular customer. </span></p>
<p><span style="font-weight: 400;">Rate limiters and sharding patterns, such as a shuffle sharding pattern, can also help reduce blast radius by containing each customer request in a particular set of resources.</span></p>
<p><img alt="" class="alignnone wp-image-7658 size-large" height="431" src="https://tyk.io/wp-content/uploads/2026/04/blog-achieve-99percent-uptime-4-1024x552.png" width="800" /></p>
<h2><span style="font-weight: 400;">Non-architectural considerations</span></h2>
<p><span style="font-weight: 400;">So many factors can cause outages. Examples include cloud providers, external vendors, internal dependent platforms, platform bugs, and untrusted code, as well as customers’ poison pill requests. It’s essential to constantly review these failure modes and convert them into “what if” scenarios. You can turn these into an SDK that converts the scenarios into an automated resiliency testing framework. </span></p>
<p><span style="font-weight: 400;">A sandbox approach for running untrusted code is also highly recommended, as is an infrastructure as code approach with shift left testing capabilities and enforcing policy as code. It means you catch problems in the CI/CD pipeline, instead of waiting for production to fail. </span></p>
<p><span style="font-weight: 400;">Release techniques are also important. With the sharding mentioned above, you can put a new release into a particular customer segment and monitor, only rolling it out more widely once you’re confident in it. This reduces failures caused by program, product, code, and configuration changes. </span></p>
<p><span style="font-weight: 400;">Deployment hooks are helpful too, with synthetic data helping to identify any configuration drift between production and non-production. Readiness checks, automated failovers, and resilience testing as code also help. </span></p>
<p><span style="font-weight: 400;">Another key factor is observability standardization, including:</span></p>
<ul>
<li style="font-weight: 400;"><span style="font-weight: 400;">Standardized logging across all services</span></li>
<li style="font-weight: 400;"><span style="font-weight: 400;">Metrics (latency, error and success rates, saturation)</span></li>
<li style="font-weight: 400;"><span style="font-weight: 400;">Thresholds with dynamic alerting</span></li>
<li style="font-weight: 400;"><span style="font-weight: 400;">Standardized error codes</span></li>
<li style="font-weight: 400;"><span style="font-weight: 400;">Distributed tracing from customer to platform</span></li>
<li style="font-weight: 400;"><span style="font-weight: 400;">KPIs</span></li>
</ul>
<p><span style="font-weight: 400;">CapitalOne uses sidecar and bulkhead patterns for observability, with sidecars for logging, observability, retries, and so on. </span></p>
<p><span style="font-weight: 400;">The result of all of this is 99.999% uptime, supporting customer trust, a competitive edge, compliance adherence, and a sound company reputation. </span></p>
<p><a href="https://tyk.io/contact/"><span style="font-weight: 400;">Speak to the Tyk team</span></a><span style="font-weight: 400;"> to find out more. </span></p>
<p>&nbsp;</p>
<p>The post <a href="https://tyk.io/blog/how-to-achieve-99-999-platform-uptime/">How to achieve 99.999% platform uptime</a> appeared first on <a href="https://tyk.io">Tyk API Management</a>.</p>
