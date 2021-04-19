# Read-17, Code 401, 19 April 2021

## AWS: API

### Review and Discussion

NOTE: I have answered these question in read-16
[Read16-link](https://omar-tarawneh.github.io/reading-notes/reading-notes-code401/read-16)

### Vocabulary

- Serverless Functions
  A serverless function is a programmatic function written by a software developer for a single purpose. It's then hosted and maintained on infrastructure by cloud computing companies. These companies take care of code maintenance and execution so that developers can deploy new code faster and easier.

- Cloud Storage
  Cloud storage involves stashing data on hardware in a remote physical location, which can be accessed from any device via the internet. Clients send files to a data server maintained by a cloud provider instead of (or as well as) storing it on their own hard drives.

- CDN
  (Content Delivery Network) is a highly-distributed platform of servers that helps minimize delays in loading web page content by reducing the physical distance between the server and the user. This helps users around the world view the same high-quality content without slow loading times.

### Preview

1. Which 3 things had you heard about previously and now have better clarity on?
   Socket io, AWS, Serverless functions, lambda functions, Cloud in general.

2. Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
   React, EC2, the difference between clouds.

3. What are you most excited about trying to implement or see how it works?
   deploy our API on the AWS Cloud.

### AWS Gateway

![gate](https://d2908q01vomqb2.cloudfront.net/1b6453892473a467d07372d45eb05abc2031647a/2018/05/23/edge-optimized.png)

Amazon API Gateway is a fully managed service that makes it easy for developers to create, publish, maintain, monitor, and secure APIs at any scale. Using API Gateway, you can create RESTful APIs and WebSocket APIs that enable real-time two-way communication applications.

API Gateway sits between the backend services of your API and your API’s users, handling the HTTP requests to your API endpoints and routing them to the correct backends. It provides a set of tools that help you manage your API definitions and the mappings between endpoints and their respective backend services. It can also generate API references from your definitions and make them available to your users as API documentation.

### AWS DynamoDB Gateway

DynamoDB is a hosted NoSQL database offered by Amazon Web Services (AWS). It offers:

reliable performance even as it scales;
a managed experience, so you won't be SSH-ing into servers to upgrade the crypto libraries;
a small, simple API allowing for simple key-value access as well as more advanced query patterns.
DynamoDB is a particularly good fit for the following use cases:

Applications with large amounts of data and strict latency requirements. As your amount of data scales, JOINs and advanced SQL operations can slow down your queries. With DynamoDB, your queries have predictable latency up to any size, including over 100 TBs!

Serverless applications using AWS Lambda. AWS Lambda provides auto-scaling, stateless, ephemeral compute in response to event triggers. DynamoDB is accessible via an HTTP API and performs authentication & authorization via IAM roles, making it a perfect fit for building Serverless applications.

Data sets with simple, known access patterns. If you're generating recommendations and serving them to users, DynamoDB's simple key-value access patterns make it a fast, reliable choice.

**Dynamoose**
Dynamoose is a modeling tool for Amazon's DynamoDB work the same as mongoose.

[GitHub-link](https://omar-tarawneh.github.io/reading-notes/reading-notes-code401/read-18)
