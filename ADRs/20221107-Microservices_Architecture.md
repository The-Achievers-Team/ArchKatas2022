Decision: We will use the microservices architecture for developing our application.

Decision Date: November 7th, 2022

Pros:

1. Scalability: Since each microservice runs independently, it is easier to add, remove, update or scale each microservice. Developers can perform these tasks without disrupting any other microservice in the system.
For our application, scalability is a key concern.

2. Elasticity: If a particular microservice experiences increased bursts of demand, more resources can be efficiently devoted to it. If demand drops, the microservice can be scaled back, allowing our application to elastic in nature.

3. Resiliency/Fault-Tolerance: With a microservices architecture, if one service fails, it’s much less likely that other parts of the application will fail because each microservice runs independently. Also, it becomes easier to perform root-cause analysis for issues, since we can isolate the independent parts of our application, identify and issue and fix it quickly without having to redeploy the whole application.

4. Deployment: A microservices architecture will let us deploy independent parts of the application without affecting other services in the architecture. This will also enable us to add new features without redesigning the complete system.


Cons:

1. Cost: While microservices architectures may save money over the long run, upfront costs may be higher.

2. Debugging and integration testing: Debugging and integration testing can be more challenging with a microservices architecture, since each microservice will have its own set of logs. This may prove to be an inconvenience when tracing the source of a problem in the code.


Justification: Scalability. elasticity, resiliency, fault-tolerance and ease of deployment are all important architectural considerations for our applications, as mentioned in the architectural-analysis section. Hence, we feel that choosing microservices architecture provides much more benefits than another architecture.
