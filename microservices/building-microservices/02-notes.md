# 1. Tips 1
If you take only one thing from this book and from the concept of microservices in general, it should be this: ensure that you embrace the concept of **independent deployability ** of your microsevices. Get into the habit of deploying and releasing changes to a single microservice in to production without having to deploy anything else. From this, many good things will follow

# 2. Key Concepts of Microservices
- Independent deployability
- Modeled around a business domain: domain-driven design
- Owning their own state: Do not share database unless you really need to, and even do everything you can to avoid it. Sharing databases is one of the worst things you can do if you are trying to achieve independent deployability
- Size: First, how many microservices can you handle? Second, how do you define microservice boundaries to get the most out of them, without everything becoming a horribly coupled mess?
- Flexibility
- Alignment of architecture and organization

# 3. Technology
- Log Aggregation and distributed tracing ([Humio](https://www.crowdstrike.com/products/next-gen-siem/falcon-logscale/), [jaegertracing](https://www.jaegertracing.io/), [servicenow](https://www.servicenow.com/products/observability.html), [honeycomb](https://www.honeycomb.io/))

- Containers and Kubernetes
- Streaming: we still need to find ways to share data between microservices ([apache kafka](https://kafka.apache.org/), [Apache Flink](https://flink.apache.org/), [debezium](https://debezium.io/))
- Public cloud and serverless

# 4. Advantages of microservices

- Technology heterogeneity, microservices can allow you to more easily embrace different technologies
- Robustness, a component of a system may fail, but as long as that failure does not cascade, you can isolate the problem, and the rest of the system can carry on working.
- Scaling, with smaller services, we can scale just those services that need scalling.
- Ease of deployment
- Organizational Alignment
- Composability

#5. Microservices pain points
- Developer Experience
- Technology overload
- Cost
- Reporting
- Monitoring and troubleshooting
- Security
- Testing
- Latency
- Data consistency