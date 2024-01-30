# Build-a-Multi-Region-Serverless-Application-for-Resilience-And-High-Availability

<img width="1316" alt="image" src="https://github.com/SwathiKrish97/Build-a-Multi-Region-Serverless-Application-for-Resilience-And-High-Availability/assets/125830594/6261192e-ae25-452e-8832-e41177f9e354">


In this workshop, we engaged in building a Customer Ticketing application using Amazon Web Services (AWS), aimed at enhancing user experience for Wild Rydes. The process involved:

Application Setup:

Enabled users to submit and monitor their support tickets.
Integrated Facebook login for user authentication.
Adopted a serverless architecture to eliminate the need for dedicated server management.
Ensured the system could switch to a backup in another location within 15 minutes during a disaster, without losing data beyond 15 minutes.

System Design:

Structured the application into three components:
A User Interface (UI) layer utilizing basic web technologies hosted on AWS S3.
An Application Programming Interface (API) layer developed in Node.js on AWS Lambda, linked through Amazon API Gateway.
A Data layer for ticket storage, implemented with Amazon DynamoDB.
Designed backend components (API, Lambda, DynamoDB) to switch to a backup location in emergencies, with DynamoDB data replicated to ensure availability.

Extra Tools:

Employed AWS Cognito for user authentication and authorization.
Utilized AWS Route53 for domain management and automatic redirection to backup locations if necessary.

Workshop Steps:

The app construction was segmented into phases:
Establishing a development environment with AWS Cloud9.
Developing the API and UI layers.
Arranging the backup infrastructure.
Conducting tests for emergency failover procedures.
Concluding the workshop with cleanup activities.
(Optional) Explored data replication across different locations and the setup of custom domain names.

Preparatory Steps:

Required an AWS account with specific service creation capabilities (IAM, S3, DynamoDB, Lambda, API Gateway).
Secured a domain name, either through purchase or existing ownership, managed directly or via AWS Route53.
