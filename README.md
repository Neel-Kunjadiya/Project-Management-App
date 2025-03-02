# Project Management Dashboard

## Overview

This repository contains the source code for a **Project Management Dashboard** built using **Next.js, Node.js, and AWS services**. Designed to streamline project tracking, task management, and team collaboration, this dashboard enhances productivity by providing real-time insights into project progress. By integrating modern web technologies such as Next.js for a dynamic user interface, Redux Toolkit for efficient state management, and AWS services for scalable backend infrastructure, this dashboard offers a seamless and intuitive user experience, ensuring efficient workflow management and accountability among team members.

## Project Overview & Impact (STAR Methodology)

**Situation**:  
Many organizations struggle with fragmented tools that hinder effective project tracking and team collaboration, resulting in reduced productivity and unclear accountability.

**Task**:  
The goal was to create a centralized dashboard that consolidates project data, streamlines task management, and facilitates real-time communication among team members.

**Action**:  
I developed this dashboard by employing a modern tech stack:
- **Frontend**: Leveraging Next.js and Tailwind CSS for dynamic, responsive interfaces, with Redux Toolkit managing state efficiently.
- **Backend**: Building a robust server using Node.js with Express, complemented by Prisma for seamless PostgreSQL integration.
- **Cloud Infrastructure**: Utilizing AWS services—including EC2, RDS, API Gateway, Amplify, S3, Lambda, and Cognito—to ensure scalability, high availability, and secure data management.

**Result**:  
The final product is a scalable, secure, and user-friendly dashboard that centralizes project management, improves team collaboration, and provides actionable insights through real-time reporting and analytics. This tool has proven invaluable in streamlining workflows and enhancing overall project execution.

## Technology Stack

The dashboard leverages a powerful and scalable technology stack to support its diverse functionality:

- **Frontend**: Next.js, Tailwind CSS, Redux Toolkit, Redux Toolkit Query, Material UI Data Grid
- **Backend**: Node.js with Express, Prisma (PostgreSQL ORM)
- **Database**: PostgreSQL, managed using PgAdmin
- **Cloud Services**: AWS EC2, AWS RDS, AWS API Gateway, AWS Amplify, AWS S3, AWS Lambda, AWS Cognito

This technology stack ensures **high performance, scalability, and security** by leveraging Next.js for fast and interactive user interfaces, Redux Toolkit for efficient state management, Node.js with Express for a robust backend, PostgreSQL for reliable data management, and AWS cloud services for high availability and protection. These components work together to maintain a modern and efficient user experience.

## Key Features

### **Project & Task Management**
- Create, update, and organize projects with tasks and deadlines.
- Assign tasks to team members and monitor their progress in real time.
- Track workflow stages with automated status updates.

### **Advanced Visualization & Collaboration**
- **Gantt Charts**: Provides interactive visual timelines for tracking project progress.
- **Collaboration Tools**: Set user permissions, share projects, and manage team roles.
- **Notifications**: Get real-time alerts on project updates, task assignments, and deadlines.

### **Security & Performance**
- **User Authentication**: Secure login and role-based access using AWS Cognito.
- **Data Security**: Ensures encrypted storage and access control measures.
- **Cloud Scalability**: Designed to handle expanding workloads without performance degradation.

### **Reporting & Insights**
- Generate reports with real-time data on project completion rates, team productivity, and workflow bottlenecks.
- Use analytics to optimize team efficiency and make data-driven decisions.

## Why This Project Matters

This **Project Management Dashboard** was developed to address inefficiencies in team coordination and workflow optimization. It provides:

- **Centralized Project Data**: Eliminates the need for multiple tracking tools, reducing complexity and improving accessibility.
- **Enhanced Team Collaboration**: Facilitates structured communication, task delegation, and accountability.
- **Better Time Management**: Helps teams prioritize tasks, avoid bottlenecks, and meet deadlines more effectively.
- **Enterprise-Ready Scalability**: Leverages cloud-native infrastructure to support teams of any size, from startups to large organizations.
- **Data-Driven Decision Making**: Empowers managers and teams with performance analytics and actionable insights.
- **Cross-Team Coordination**: Enables multiple teams to work in parallel with full visibility into shared and interdependent projects.

This dashboard is ideal for **project managers, software development teams, marketing teams, and organizations** that require a structured and scalable approach to managing their projects. **Project managers** can streamline workflows and track deliverables with real-time insights. **Software development teams** benefit from enhanced collaboration features, ensuring smooth sprint planning and task allocation. **Marketing teams** can efficiently coordinate campaigns, track deadlines, and manage resources. **Organizations** of all sizes gain a centralized platform to oversee multiple projects, improving visibility, accountability, and team productivity.

## Prerequisites

To set up and use this system effectively, install the following tools:

- **Git** (for version control and collaboration)
- **Node.js** (to run the backend and frontend applications)
- **npm** (Node Package Manager, to install project dependencies)
- **PostgreSQL** (to manage and store database records)
- **PgAdmin** (for managing the PostgreSQL database with a graphical interface)

### Database Management Command

If needed, use this SQL command to reset primary key sequences in the database:
```sql
SELECT setval(pg_get_serial_sequence('"[DATA_MODEL_NAME_HERE]"', 'id'), coalesce(max(id)+1, 1), false) FROM "[DATA_MODEL_NAME_HERE]";
