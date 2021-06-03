

# Amazon SNS 

## SNS-Amazon Simple Notification Service

 a managed service that provides message delivery from publishers to subscribers 


## Features 
SNS provides the following features:

- Application-to-application messaging
- Application-to-person notifications
- Standard and FIFO topics
- Message durability 
- Message archiving and analytics
- Message attributes
- Message filtering
- Message security

##  Amazon SNS services:
- `Amazon SQS`
a secure, durable, and available hosted queue that lets you integrate and decouple distributed software systems and components.
1. Amazon SNS provides dead-letter queues powered by Amazon SQS for undeliverable messages.
2. You can subscribe an Amazon SQS queue to an SNS topic.
3. You can subscribe an Amazon SQS FIFO queue to an Amazon SNS FIFO topic to receive messages in order and with no duplicates.
- `AWS Lambda`
 enables you to build applications that respond quickly to new information.
- `AWS Identity and Access Management (IAM)`
securely control access to AWS resources for your users. Use IAM to control who can use your Amazon SNS topics (authentication)
- `AWS CloudFormation`
model and set up your AWS resources. Create a template that describes the AWS resources that you want, including Amazon SNS topics and subscriptions. 

## Accessing Amazon SNS
configure and manage SNS topics and subscriptions using: 
- Amazon SNS console
provides a convenient user interface for creating topics and subscriptions, sending and receiving messages, and monitoring events and logs.
-  command line tools
The AWS Command Line Interface (AWS CLI) gives you direct access to the Amazon SNS API for advanced configuration and automation use cases.
 - AWS SDKs.


