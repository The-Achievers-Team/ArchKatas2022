
# Security

Our application needs to have security built-in, at both infratructure level, and application level. The following security considerations are the most important but not exhaustive:

## Authentication & Authorization

Authentication and authorization for users of the application will be done using the microservice "Authentication & Registration", and access will be granted to backend mciroservices and APIs based upon user roles.

Authentication and authorization for development and deployment can be accomplished using the solution and services already being used by the HeyBlue team. For e.g. - if AWS is being used by HeyBlue team to develop and deploy their applications, the following AWS services can be used to control access to AWS cloud resources:

- IAM (AWS Identity Access Management) - for provisioning access to AWS services for development and deployment
- SSO (Single Sign On) - If a single sign on solution such as Okta is being used by HeyBlue team, it can be integrated with AWS IAM to provide a secure and seamless experience for the development team.

## Network & Infrastructure Security

It is important to secure network and infrastructure on which our application will be deployed and run.

For network traffic, it is important to ensure that microservices are deployed within a private network which are accessible only from the public API gateways, Furthermore, it is important to only open system ports on which our microservices will listen.

Folowing types of solutions should be deployed to monitor and filter public traffic to our API gateways:

- DDoS protection
- Web Application Firewall
- Network Firewall

Furthermore, system components such as underlying operating systems, containers, orchestration systems (such as Kubernetes) should be hardened according to benchmark guidelines to ensure security of the application.

## Data Security

All traffic to our application and within our infrastrcuture should be encrypted in transit using SSL/TLS. SSL/TLS should be enabled in a secure manner, only allowing secure SSL/TLS versions and secure ciphersuites.

All data at rest (databases) should be encrypted using data-at-rest encryption technologies. Most cloud providers provide out-of-the box data-at-rest solutions for storing data.

Salted hashes should be used for storing passwords, and the application should enforce strong password requirements.

Secrets during development/deployment (API keys, certificates, passwords) should be secured using a secrets-management tool of choice.

## Threat Detection & Monitoring

Application and system logs such as API gateway logs, microservices (container) logs, OS logs, orchestration tool (e.g. - kubernetes) logs should be sent to a centralized logs aggregating, threat detection and monitoring tool, where rules are created to monitor and alert upon suspicious activity.

