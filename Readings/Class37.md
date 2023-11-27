## S3 Storage

- Introduction to Amazon S3:
Amazon S3 (Simple Storage Service) is a scalable object storage service offered by Amazon Web Services (AWS). It allows users to store and retrieve any amount of data from anywhere on the web.

- Features of Amazon S3:
1. Scalability: S3 scales automatically to handle varying levels of data and traffic.
2. Durability and Reliability: S3 is designed for 99.999999999% durability, and it redundantly stores data across multiple facilities and devices.
3. Security and Access Management: S3 provides features like bucket policies, access control lists (ACLs), and encryption to control access to your data.

- Object Key in Amazon S3:
An object key is a unique identifier for an object within an S3 bucket. It is composed of a prefix and an object name, and it serves as the unique address for accessing the object within the bucket.

- S3 with Amplify:
Dependencies for Amplify AWS S3 in Android:
`implementation 'com.amplifyframework:core:1.0.0'`
`implementation 'com.amplifyframework:aws-storage-s3:1.0.0'`

- To upload data to your S3 bucket using Amplify, you need to configure Amplify with your AWS credentials and set up an S3 bucket. Ensure that the appropriate IAM (Identity and Access Management) policies are set for the credentials used.

- Initializing Amplify Auth and Storage:
In Amplify, the Amplify library needs to be initialized with the necessary categories. For Auth and Storage, you can use the following methods:

### Initialize Amplify Auth
`Amplify.addPlugin(new AWSCognitoAuthPlugin());`
`Amplify.configure(getApplicationContext());`

### Initialize Amplify Storage
`Amplify.addPlugin(new AWSS3StoragePlugin());`
`Amplify.configure(getApplicationContext());`