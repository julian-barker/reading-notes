[Home](../README.md)

# Class 18

## AWS Cont'd

### AWS API Gateway

- API Gateway is a managed service that allows you to connect HTTP or WebSocket API endpoints with backend functionality without maintaining an API server.
- Since you do not need to maintain a server, you need a way for your endpoints to trigger functions and data fetching, and that is what API Gateway gives you.
- API Gateway integrates with AWS Lambda, AWS SNS, and Amazon Cognito
- API Gateway has several benefits:
  - Maps HTTP/REST requests and Websocket events to serverless functions
  - Allows you to use several different functions to serve the same top-level API, allowing for encapsulation of logic
  - Easy integration with other AWS services.

### AWS DynamoDB

- DynamoDB is a NoSQL database
- It is particularly well-suited for large quantities of data and applications requiring low latency
- It also integrates easily with Lambda serverless functions
- It works well for datasets with simple and known access patterns
- I would recommend DynamoDB over MongoDB if you are already using AWS Lambda functions.
- DynamoDB is a fast NoSQL database that offers 25GB of free storage and up to 200M read/writes per month on the AWS Free tier. It is a key-value store database, meaning it operates similarly to objects or maps in JS. It offers built-in security, in-memeory cacheing for repeated requests, automatic backups, and tools to help you import and export your data.

### Dynamoose

- Dynamoose is essentially to DynamoDB what Mongoose is to MongoDB. From the Dynamoose site, it has the following key features:
  - Type safety
  - High level API
  - Easy to use syntax
  - DynamoDB Single Table Design Support
  - Ability to transform data before saving or retrieving items
  - Strict data modeling (validation, required attributes, and more)
  - Support for DynamoDB Transactions
  - Powerful Conditional/Filtering Support
  - Callback & Promise support
  - AWS Multi-region support
