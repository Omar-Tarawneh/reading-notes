# Read-19, Code 401, 21 April 2021

## Review and Discussion

NOTE: I have answered these question in read-16
[Read16-link](https://omar-tarawneh.github.io/reading-notes/reading-notes-code401/read-16)

## Vocabulary

- Serverless API
  Serverless is a cloud computing execution model where the cloud provider dynamically manages the allocation and provisioning of servers. A serverless application runs in stateless compute containers that are event-triggered, ephemeral (may last for one invocation), and fully managed by the cloud provider.

- Triggers
  A trigger is a special type of stored procedure that automatically runs when an event occurs in the database server. DML triggers run when a user tries to modify data through a data manipulation language (DML) event. DML events are INSERT, UPDATE, or DELETE statements on a table or view

- Dynamo vs Mongo
  MongoDB is vendor agnostic, Open Source, and can be deployed anywhere. DynamoDB is only available on AWS.
  DynamoDB is a fully managed AWS service, MongoDB can be self installed or fully managed with MongoDB Atlas.
  DynamoDB as an integrated AWS service makes it easier to develop end to end solutions.
  DynamoDB uses tables, items and attributes, MongoDB uses JSON-like documents.
  DynamoDB supports limited data types and smaller item sizes; MongoDB supports more data types and has fewer size restrictions.

- Dynamoose vs Mongoose
  DynamoDB is a key-value store with added support for JSON to provide document-like data structures that better match with objects in application code. ... Compared to MongoDB, DynamoDB has limited support for different data types. For example, it supports only one numeric type and does not support dates.

## Preview

1. Which 3 things had you heard about previously and now have better clarity on?
   AWS in general, Auth, Socket io
2. Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
   we Take about the routes and serverless API
3. What are you most excited about trying to implement or see how it works?
   Try to do a serverless API.

### AWS SQS & SNS

SQS: Amazon Simple Queue Service (Amazon SQS) is a reliable, highly-scalable hosted queue for storing messages as they travel between applications or microservices. Amazon SQS moves data between distributed application components and helps you decouple these components.

For information on the permissions you need to use this API, see Identity and access management in the Amazon Simple Queue Service Developer Guide.

You can use AWS SDKs to access Amazon SQS using your favorite programming language. The SDKs perform tasks such as the following automatically:

Cryptographically sign your service requests

Retry requests

Handle error responses

SNS: Amazon Simple Notification Service (Amazon SNS) is a web service that enables you to build distributed web-enabled applications. Applications can use Amazon SNS to easily push real-time notification messages to interested subscribers over multiple delivery protocols. For more information about this product see the Amazon SNS product page. For detailed information about Amazon SNS features and their associated API calls, see the Amazon SNS Developer Guide.

For information on the permissions you need to use this API, see Identity and access management in Amazon SNS in the Amazon SNS Developer Guide.

We also provide SDKs that enable you to access Amazon SNS from your preferred programming language. The SDKs contain functionality that automatically takes care of tasks such as: cryptographically signing your service requests, retrying requests, and handling error responses. For a list of available SDKs, go to Tools for Amazon Web Services.

[GitHub-link](https://omar-tarawneh.github.io/reading-notes/reading-notes-code401/read-19)
