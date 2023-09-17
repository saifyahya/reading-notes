## Spring Security

- **Authentication**
 refers to the process of verifying the identity of a user, typically by confirming that the user is who they claim to be. It involves validating user credentials, such as username and password, against a trusted source, such as a database or an identity provider. The goal of authentication is to establish the user's identity with a reasonable degree of certainty.
 - **Authorization** 
  is the process of determining what actions or resources a user is allowed to access or perform after they have been authenticated. Once a user's identity is established, authorization determines the permissions or privileges associated with that identity. It specifies what the user can or cannot do within an application or system.

  - Outcomes of the *AuthenticationManager's* `authenticate()` method are:

a. It can return an Authentication object with authenticated set to *true*, indicating that the input provided by the user represents a valid principal. This means the user has been successfully authenticated.

b. It can throw an *AuthenticationException* if it believes that the input provided represents an invalid principal. This occurs when the user's credentials are incorrect or authentication fails for some other reason.

c. It can return *null* if it cannot make a definitive decision regarding the authentication. This outcome typically means that the AuthenticationManager is unable to verify the user's identity based on the provided input, and further processing or checks may be required.