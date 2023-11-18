## Amplify and Cognito 

- Where in your application should you check the current auth session?

You should check the current auth session when it is relevant to your application's logic, typically during the initialization or at a point where user authentication status is critical. In the provided example, it suggests testing purposes by running the check in the onCreate method of the MainActivity. Depending on your application's requirements, you might want to check the auth session at different points, such as when a user navigates to a secure section of your app.
What is the command that is used to push your changes to the cloud?

- The command used to push your changes to the cloud is:

amplify push
This command deploys your backend resources, including the authentication configuration, to the cloud.

- What does Amplify Auth do for your application?

Amplify Auth provides an interface for authenticating users in your application. It abstracts away the complexity of user authentication by integrating with authentication providers like Amazon Cognito User Pool and Identity Pool. It allows you to easily set up authentication in your application using Amplify CLI or Amplify Studio console. Amplify Auth also manages authentication sessions, allowing you to check the current auth session, and provides options for customization and advanced configuration if needed. Additionally, it seamlessly integrates with other Amplify categories, providing necessary authorization across your application.