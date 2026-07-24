---
title: "GreenLens Project Development Process"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 5.1. </b> "
---

#### Overview

The GreenLens project was developed by a team of four members. Vinh served as the team leader and was responsible for the backend development, core business logic, AWS account management, AWS services configuration, and deployment of the system to AWS. Loi also contributed to the backend work, while Phuc and I were responsible for frontend development.

#### Note

This section summarizes the project development process and team workflow used during the GreenLens project. It is structured as a report-style chapter so it can be inserted into the Workshop content consistently.

#### Content
1. [Introduction](#1-introduction)
2. [Project Preparation](#2-project-preparation)
3. [Task Planning and Work Organization](#3-task-planning-and-work-organization)
4. [Frontend Development](#4-frontend-development)
5. [Backend Development](#5-backend-development)
6. [AWS Setup and Deployment](#6-aws-setup-and-deployment)
7. [Testing and Integration](#7-testing-and-integration)
8. [Collaboration and Source Control](#8-collaboration-and-source-control)
9. [Final Review and Handover](#9-final-review-and-handover)
10. [Conclusion](#10-conclusion)

## 1. Introduction

GreenLens was built as a collaborative project with clearly defined responsibilities for each member. The project ran from June 1, 2026 to July 6, 2026 and followed a structured workflow from requirement analysis and task planning to development, testing, and final deployment.

## 2. Project Preparation

At the beginning of the project, the team reviewed the requirements and discussed the overall direction of the website. This preparation stage helped us define the scope of work, understand the expected functionality, and align the team before implementation began.

- Backend development, business logic, AWS management, and deployment were assigned to Vinh and Loi.
- Frontend development was assigned to Phuc and me.
- All tasks were created and tracked on Jira.
- The source code was managed on GitHub to support collaboration and version control.

By separating responsibilities early, the team was able to work in parallel and avoid confusion during later stages of development.

## 3. Task Planning and Work Organization

The project work was broken down into smaller tasks and recorded in Jira. Each task contained a clear description, an assigned owner, and a status so the team could monitor progress throughout the project. This helped us keep the work organized, identify blockers early, and ensure that no important feature was missed.
GitHub was used as the main source code repository. Team members committed code according to the assigned tasks, which made it easier to review changes, manage versions, and integrate frontend and backend updates consistently.

## 4. Frontend Development

Phuc and I focused on the frontend part of the system. Their work included building the user interface, implementing the main pages, handling interactions, and connecting the UI to backend APIs. The frontend was developed in parallel with the backend so that the interface and server logic could be aligned continuously.
During this phase, the team paid attention to usability and consistency so the website could provide a clear and smooth experience for users.

## 5. Backend Development

On the backend side, Loi and Vinh developed the core logic of the project and implemented the APIs used by the frontend. This included handling business rules, processing requests, returning responses, and making sure the data flow between the client and server remained correct and reliable.
In addition to the application logic, Vinh also managed the AWS account and configured the AWS services required by the project. This ensured the backend could be deployed and operated in a stable cloud environment.

## 6. AWS Setup and Deployment

After the main features were completed, the system was prepared for deployment on AWS. Vinh was responsible for setting up the cloud environment, configuring the necessary services, and deploying the application so the website could run in a production-like environment.
This deployment stage was essential because it transformed the project from a local development solution into a cloud-hosted system that could be accessed and tested more realistically.

## 7. Testing and Integration

Once the frontend and backend were connected, the team performed integration testing to verify that the components worked together correctly. We checked the main user flows, reviewed the communication between frontend and backend, and fixed issues discovered during testing.

- Functionality was tested end to end.
- Integration between frontend and backend was verified.
- Issues found during testing were logged and fixed through Jira tasks.

This stage helped improve stability and ensured the system was ready for final delivery.

## 8. Collaboration and Source Control

Throughout the project, Jira and GitHub played a central role in team coordination. Jira helped us track progress and assignments, while GitHub provided a safe and transparent way to manage source code. Together, these tools made collaboration easier and reduced the risk of overlap or lost changes.

## 9. Final Review and Handover

Before closing the project, the team performed a final review of the implemented features, checked the deployment status on AWS, and verified that the most important user flows worked as expected. This final review helped confirm that the project was ready for handover and presentation.
The project documentation, source code repository, and task history were kept organized so that the system could be maintained and extended in the future. This also made it easier to review the development process and explain how each part of the system was built.

## 10. Conclusion

Overall, the GreenLens project was completed through a clear and well-organized workflow. The team worked with defined responsibilities, maintained consistent communication, and used Jira and GitHub effectively to manage tasks and source code. As a result, the project was developed successfully within the planned timeline from June 1, 2026 to July 6, 2026.

GitHub: [GreenLens repository](https://github.com/2280603697NguyenQuangVinh/Greenlens)
Live demo: [GreenLens deployment](https://main.d32rydccx28td4.amplifyapp.com/)
