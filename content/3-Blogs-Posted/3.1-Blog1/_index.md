---
title: "Blog 1"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 3.1. </b> "
---
# The process of refining the Serverless architecture for the GreenLens Kids project through practical experience*

Hello everyone, we are the We Are One team participating in AWS’s First Cloud AI Journey. Today, I want to share some real-world lessons we learned while designing the system architecture for GreenLens Kids. This project was built on AWS Serverless, applied AI, and gamification to guide children in sorting waste.

Below are the key lessons our team distilled after technical review sessions with mentors and refining our initial architecture diagram.

---

## 1. Hidden security risk behind optimizing user experience

To make the app as easy as possible for children, our team initially decided to skip login. However, mentors identified a critical vulnerability. Without authentication, endpoints — especially the AI Camera — become easy targets for abuse or denial-of-service attacks. The consequence could be rapid exhaustion of our AWS resource budget. To fix this, we implemented AWS Cognito Guest Access to safely identify devices and added AWS WAF behind API Gateway to control traffic and block malicious requests.

---

## 2. Fixing fragmentation in data flow planning

In the initial architecture, our Lambdas were scattered and mainly just connected to S3. The operational management flow was also completely separated from the shared database, making the entire system inconsistent. Thanks to detailed expert reviews, we restructured the entire diagram into proper layers for easier management and scalability: Presentation Layer, API Layer, Application Layer, Data Layer, and AI Services.

---

## 3. Understanding the orchestration behavior of AWS services

In the early version, we designed a flow where Amazon Rekognition and Amazon Bedrock interacted directly, and we also inserted Amazon ElastiCache into the flow in an unsuitable way. After reviewing the technical documentation carefully, we decided to streamline the system. AWS Lambda was returned to its proper role in a Serverless event-driven architecture, acting as the central logic coordinator between the application and external AI services.

---

## Lessons learned and conclusion

Through continuous iteration, fixes, and refinement, our team came to realize that architecture design is not just about connecting services to satisfy functionality. The core and most challenging problem is finding the right trade-off between user experience, cost optimization, and system security limits.

Special thanks to the First Cloud AI Journey organizers and mentors who followed our project closely. Their rigorous but practical reviews helped our team strengthen our thinking foundation and feel more confident and ready for future real-world projects.
![alt text](../architecture.png)