[Home](../README.md)

# Class 19

## AWS Cont'd (SNS & SQS)

- SNS stands for Simple Notification System. It is a publish-subscribe service that pushes messages to subscribed entities as they are produced by a publisher. It is capable of pushing messages to various devices and operating systems, such as iOS, Android, and Google.
  - SNS uses a push mechanism where publishers push messages to subscribers.
  - SNS does not retain messages if no consumer is available, and so does not guarantee message delivery.
  - All consumers are expected to process messages in different ways.

- SQS stands for Simple Queue Service. It is a queueing system that allows the sending of messages between components and services in a FIFO manner, allowing for loose coupling of components in a microservice architecture.
  - SQS uses a pull mechanism where consumers poll for messages from SQS.
  - SQS guarantees message delivery due to message retention.
  - All consumers are supposed to be processing the message in the same way.

- Both services can be used together in a fanout pattern in which SNS distributes the same message to multiple different SQS queues.
- Push notifications work through publishing events, which subscribers are listening for.
- SQS can be used in large scale, distributed applications to serve as the communication layer between components or services, which allows them to function relatively independent of one another.
