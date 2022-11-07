Decision: We will use API gateways in our application for routing requests to backend microservices.

Pros:

1. Security: Since API gateways sit between your front end applications and the microservices, it will act as a security barrier making sure your sensitive API Endpoints are not exposed. API gateways provide important functionality such as rate-limiting, authentication and access-control, scaling. They will protect our backend APIs from malicious attack vectors such as DoS attacks, SQL injections, and other several other similar attacks that may take advantage of our backend API’s vulnerabilities.

2. Decreased Microservices Complexity: Since the API gateways can manage important features mentioned above, our applications backend microservices do not have to implement all these features individually, and can focus on impleneting the business functionality.

3. Monitoring and Analytics: API gateways come with monitoring and analytics tools and integrations, which we can use to monitor and analyze the traffic to our application.

Cons:

1. Single point of failure: API gateways can become a single of failure, if careful consideration is not paid to how we implement and monitor them.

2. Complexity: Complexity is also increased since it is an additional infrastructure component that the development team has to learn about and maintain.

Justification: We feel that the benefits provided by API gateways are much more important than the drawbacks, and the cons can be handled with careful implementation.