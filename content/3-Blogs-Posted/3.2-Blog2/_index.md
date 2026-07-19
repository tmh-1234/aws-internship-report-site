---
title: "Blog 2"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 3.2. </b> "
---
# Building the Cloud Application Layer with First Cloud AI Journey

Although we already had an information technology foundation from our university training, facing the challenge of deploying a serverless system on AWS still felt unfamiliar and difficult. Through the First Cloud AI Journey program, our team, We Are One, had the opportunity to move from dry classroom theory to a real cloud project with many challenging problems.

## 1. Building the foundation from the very first steps

Our journey did not begin with complex code, but with getting familiar with the AWS ecosystem. The first few days were full of difficulties while setting up an AWS Free Tier account. We even had to create support cases to resolve issues with phone number verification and payment card authentication.

The team studied the modules in the AWS Study Group and completed a series of AWS SimuLearn labs, from Cloud Computing Essentials and NoSQL Database to Core Security Concepts. This process helped us complete all 12 labs and earn the AWS Cloud Practitioner certificate, which became a solid stepping stone toward the application layer.

## 2. Moving into the application layer and solving local architecture problems

Instead of working only in the Console, we began to research more deeply into the FastAPI architecture combined with AWS and set up a cloud-simulation solution directly on local machines. New knowledge was continuously applied, such as building an optimized Dockerfile and configuring `docker-compose.yml` to integrate a DynamoDB Local container.

We also learned how to set up Docker networking and Docker volumes to store database data persistently. Along with that, we managed environment variables securely and used the Boto3 library to write code for connecting systems and designing data schemas for key processing flows such as XP scoring and user status updates. This process helped the whole team understand how a backend application communicates with cloud infrastructure, how to package an application, and how to think about standardized data.

## 3. Overcoming real-world incidents

Doing a project also means dealing with unexpected risks. One memorable incident happened when the API system suddenly stopped responding. After analyzing the issue, the team discovered that the main AWS account had run out of Free Credit. We had to quickly create a new cloud environment, reconfigure IAM permissions, move the infrastructure resources, and fix the resulting Access Denied errors.

In addition, we spent a lot of time debugging issues such as character state not syncing between DynamoDB and the application interface, or incorrect JSON formatting between the backend and frontend.

## 4. Improving the user experience with AI services

The learning process during FCAJ reached a more mature stage when the team began integrating AI services into the workflow. In the AI Camera feature, we not only handled image recognition logic but also worked closely with the frontend team to improve UX. Specifically, we supported mapping complex data from the backend to the result screen interface.

We also proposed and successfully integrated the Web Speech API to create a voice for the mascot, automatically combining recycling guidance text to read the results aloud for children. Dynamically rendering educational content cards about environmental impact based on the returned JSON data was also handled smoothly.

## Conclusion

The First Cloud AI Journey program did not just provide resources; it created an environment where the team could apply knowledge in practice. From students who were only used to coding on personal computers, we learned how to design architecture, handle infrastructure issues, and integrate AI to solve a complete environmental education problem. We would like to sincerely thank the organizers and the mentors for creating such a valuable learning opportunity.
