Decision: We will create a separate microservice for authentication and authorization, instead of using API gateway for authentication/authorization.

Decision Date: November 7th, 2022

Pros:

1. Consistency: Since we are using different API gateways for browser and mobile users, abstracting authentication/authorization in a different microservice will improve consistency for authentication/authorization functionality, and reduce chance of mis-configurations/errors in implementation.

2. RBAC: Our applications has different types of users (civilians, police-officers, charities, retail-stores). Each of these users need to access to only certain parts of the application (or certain microservices in the backend). Having full control over how to implement authentication/authorization and not using an out-of-the solutions provide by API gateways for authentication/authorization will make it easier to develop custom RBAC solution for authorization.

Cons:

1. Cost: Having a separate microservice instead of using an out-of-the box solution provided by API gateways is more costly in terms of development and maintainence.


Justification: We feel that the pros are important enough to justify our decision.
