Decision: Use 2 API gateways, one for each of browser users and mobile users.

Pros:

1. Extensability: Our API Gateway service will be growing and evolving based on different requirements from both the browser and mobile client-applications. It's better to split the API Gateway in 2 API Gateways to better serve the requirements of both client applications, and extend them separately based on the different needs of both rtypes of clients.

2. De-coupling: Having a single API gateway for both browser abd mobile clients will make it act like a monolithic aggregator/orchestrator, and violate microservice autonomy by coupling all the microservices.

Cons: 

1. Debugging and monitoring: Having 2 different API gateway may make it harder to debug issues and monitor the application.

Justification: We feel that de-coupling and extensability are very important factors for our application, and the pros outweigh the cons.