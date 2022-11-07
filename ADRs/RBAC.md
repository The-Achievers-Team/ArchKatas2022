Decision: Authentication + Registration microservice will implement role based access control mechanism, since we need to support multiple types of users: civilians, police-officers, charities, retail-stores. The microservice will generate session tokens for each user, include and the role information in the session tokens (it will fetch the role information from authentication database), and grant access to backend microservices and APIs based off of the information contained in the session token.

Pros:

1. Access Control: Access will be restricted to backend microservices, and will only be granted according to the role assigned to each user.

2. Extensability: Additional roles can be added easily later on, if there is a new type of user.

3. Security and compliance: It will result in improved security and compliance, since it allows the team to view access control policies and monitor access issues in a single view.


Cons:

1. Complexity: Maintaining multiple roles may result in increased complexity.

2. Stale policies: Access control policies will need to be kept upto date, everytime we add/delete a microservice/API from the backend (which won't be that often).


Justification: Access control based on roles is an absolutely essential security feature for our application since we need to support multiple types of users as mentioned above.