# GLU02-AWS100 - Introduction to SNS (Simple Notification Service)

## Cloud Service Provider
- Amazon Web Services

## Difficulty
- Level 100 (Introductory)

## Project's Author(s)

- [Edward Allen Mercado](https://twitter.com/edwardmercado_)

## Architecture 
<p align="center">
  <img src="https://user-images.githubusercontent.com/80279467/177027784-09d439af-035d-4195-9bf4-54b4c8cb4508.png">
</p>

### You need to complete the following:

- Create an SNS topic
- Subscribe to that SNS topic with an email address of yours
- Make sure to accept the subscription in the email you receive
- Send a test message through the SNS topic
- Make sure you received the message to your email address

### You need to answer the following:

## - What is Simple Notification Service (SNS)?
Amazon Simple Notification Service is a notification service provided as part of Amazon Web Services since 2010. It provides a low-cost infrastructure for mass delivery of messages, predominantly to mobile users. 

## - How do Pub/Sub notifications work?
Publish/subscribe messaging, or pub/sub messaging, is a form of asynchronous service-to-service communication used in serverless and microservices architectures. In a pub/sub model, any message published to a topic is immediately received by all of the subscribers to the topic.

## - What are the different endpoints that SNS can send notifications to?
You can use Amazon SNS to send notification messages to one or more HTTP or HTTPS endpoints. When you subscribe an endpoint to a topic, you can publish a notification to the topic and Amazon SNS sends an HTTP POST request delivering the contents of the notification to the subscribed endpoint.

## - What happens if a message or notification in SNS cannot be delivered?
Amazon SNS defines a delivery policy for each delivery protocol. The delivery policy defines how Amazon SNS retries the delivery of messages when server-side errors occur (when the system that hosts the subscribed endpoint becomes unavailable). When the delivery policy is exhausted, Amazon SNS stops retrying the delivery and discards the message—unless a dead-letter queue is attached to the subscription. For more information, see Amazon SNS dead-letter queues (DLQs).

## - What's the difference between Simple Notification Service (SNS) and Simple Queue Service (SQS)?
In simple terms, SNS - sends messages to the subscriber using push mechanism and no need of pull. SQS - it is a message queue service used by distributed applications to exchange messages through a polling model, and can be used to decouple sending and receiving components.

## Reference

- [AWS SNS Official Documentation](https://docs.aws.amazon.com/sns/latest/dg/welcome.html)
- [Setting Up Amazon SNS Notifications](https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/US_SetupSNS.html)
- [Amazon SNS (from AWS) - The Ultimate Guide](https://www.serverless.com/amazon-sns)
- [What is Amazon SES and SNS in AWS?](https://intellipaat.com/blog/what-is-amazon-ses-sns-in-aws/)

## Costs

- Included in the Free Tier

## Estimated time to complete

- 30 minutes

