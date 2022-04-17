# [Reading-Notes](https://alsosteve.github.io/reading-notes/)
code fellows 401

# Read: 19 - AWS: Events

## Describe the similarities between AWS API Gateway + Lambda functions and an ExpressJS Server
All can be used in the WRRC cycle

## List the AWS Database offerings and talk about the pros and cons of each
- Key-value: High-traffic web apps, e-commerce systems, gaming applications
- In-memory: Caching, session management, gaming leaderboards, geospatial applications
- Document: Content management, catalogs, user profiles
- Wide-column: High scale industrial apps for equipment maintenance, fleet management, and route optimization
- Graph: Fraud detection, social networking, recommendation engines
- Time series: IoT applications, DevOps, industrial telemetry
- Ledger: Systems of record, supply chain, registrations, banking transactions

## What’s the difference between a FIFO and a standard queue?
Standard queues provide at-least-once delivery, which means that each message is delivered at least once. FIFO queues provide exactly-once processing, which means that each message is delivered once and remains available until a consumer processes it and deletes it

## How can the server be assured a message was properly received?
Request and response

## Vocab:

Serverless API: a cloud computing execution model where the cloud provider dynamically manages the allocation and provisioning of servers

Triggers: the method of embedding information in the document that tells the javascript where to attach its event handlers

Dynamo vs Mongo: Both are databses, Dynamo is for AWS and mongo is for local storage

Dynamoose vs Mongoose: Modeling tool for the DynamoDB and MongoDB
