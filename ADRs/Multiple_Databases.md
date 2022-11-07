Decision: Use separate database(s) per microservice.

Pros:

1. Standard Apporoach for microservices : By definition, microservices should be loosely coupled, scalable, and independent in terms of development and deployment. Therefore, the database per service is a preferred approach as it perfectly meets those requirements.

2. Resiliency: Changes to an individual database don’t impact other services. Hence, single points of failures are reduced.

3. Scalability: Individual data stores are easier to scale.

4. Simplicity: Since microservices should be independent in terms of development, having separate databases makes easier to understand the service with its data, making it simple to develop and maintain.

Cons:

1. Cost: Cost of maintaining multiple databases is higher than using a single database, as more number of replicas and backups will need to be maintained.

2. Data Duplication: There might be some data duplication across databases in different microservices.

3. Data Consistency and Atomicity: It may be hard to maintain data consistency and atomicity for complex queries across microservices/databases, where results of an operation in one microservice/database feed into another microservice/database.

Justification: Ultimatley we feel that the pros are more important according to our architecure points of concern. And there are workarounds for the cons, such as making sure we do not mix the data across databases to reduce data duplication and maintain data consistency and atomocity.