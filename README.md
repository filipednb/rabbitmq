# RabbitMQ

In this repository we'll see how to implement RabbitMQ into a Java Application
according to [Java Client API](https://www.rabbitmq.com/api-guide.html).

## Message Queue Concept

A message queue is a form of asynchronous service to service communication used
in serverless and microservices architectures. Messages are stored on the *queue*
until they are processed and deleted. Each message is processed only once, by
a single consumer.

### Advantages
- The message queues could simplify the development of applications that
needs to communicate asynchronously with each other. 
- There are no direct connections between applications, so it promotes 
the decoupling as seen in common coupled applications that uses HTTP-API 
communication.
- Promotes the single responsibility of applications and microservices 
architecture.
- Promotes the improving of scalability, as it enable us to decouple 
different parts of our application and then scale them independently.
- Promotes resiliency. By splitting our app in different components by queues, 
we inherently create more resiliency. Our application can still be operational 
even if some component became unavailable.
- Better monitoring, message queues components enable us to easily monitor 
how many items are in a queue, the rate of processing messages, 
and other stats.

## What is RabbitMQ?

RabbitMQ is a open source software that implements the Advanced Message Queueing
Protocol ([AMQP](https://www.amqp.org)). This protocol is an open standard
for passing business messages between applications. It could connect different
systems built with different programming languages.
