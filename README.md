# Question Setting Platform

## Overview  
The Question Setting Platform is a full-stack application designed to streamline the process of creating, managing, and distributing examination questions. It includes separate functionalities for educators, administrators, and reviewers. The platform ensures a seamless experience from question creation to review and distribution, with real-time updates and efficient management of question banks and assessments.  

---

## Features  

### *Educator Functionality:*  
- Register, login, and manage personal profiles.  
- Create and customize questions across various subjects and difficulty levels.  
- Submit questions for review and approval.  
- Access history of created questions and receive feedback.  

### *Admin Functionality:*  
- Manage users (educators and reviewers) and question banks.  
- Monitor question submissions and approve or reject questions.  
- Oversee platform-wide activities and generate reports.  
- Access platform analytics for performance and quality checks.  

### *Reviewer Functionality:*  
- View assigned questions and provide reviews or suggestions.  
- Approve or reject questions based on predefined guidelines.  
- Access review history and quality metrics.  

---

## Technology Stack  
- *Backend:* Node.js, Express.js  
- *Frontend:* React.js, Tailwind CSS  
- *Database:* MongoDB  
- *Authentication:* JWT for secure role-based access control  

---

## Requirement Analysis  

### *Stakeholder Needs:*  

#### *Educators:*  
- Easy registration and login.  
- A user-friendly interface to create and manage questions.  
- Real-time updates on question approval status.  

#### *Admins:*  
- Tools for managing users and question banks.  
- Oversight of platform compliance and activity.  
- Access to analytics and performance reports.  

#### *Reviewers:*  
- A system to review and provide feedback on submitted questions.  
- Tools to ensure quality control of questions.  

### *Platform Requirements:*  
- Secure authentication and role-based access control.  
- Scalable backend to handle increasing users and questions.  
- Efficient data management for question banks and reviews.  

---

## Functional Requirements  
- User registration and secure role-based authentication.  
- CRUD operations for questions, users, and reviews.  
- Real-time updates for question review status.  
- Advanced filtering and search for questions and user management.  

## Non-Functional Requirements  
- High scalability to support growing user base.  
- Reliable performance with minimal downtime.  
- Secure handling of sensitive data (e.g., user profiles, question banks).  
- Intuitive and responsive UI/UX design.  

---

## API Documentation  

### *Authentication Endpoints*  

#### *Educator Authentication:*  
- POST /educator-register: Register a new educator.  
- POST /educator-login: Login for educators.  
- POST /educator-logout: Logout from the platform.  

#### *Reviewer Authentication:*  
- POST /reviewer-register: Register a new reviewer.  
- POST /reviewer-login: Login for reviewers.  
- POST /reviewer-logout: Logout from the platform.  

#### *Admin Authentication:*  
- POST /admin-register: Register a new admin.  
- POST /admin-login: Login for admins.  
- POST /admin-logout: Logout from the platform.  

### *Question Management Endpoints (Educators)*  
- POST /create-question: Add a new question.  
- POST /update-question: Update question details.  
- POST /delete-question: Remove a question from the platform.  
- GET /questions: Retrieve all questions.  

### *Review Management Endpoints*  

#### *Educators:*  
- POST /submit-question: Submit a question for review.  
- GET /review-status/:id: Check the status of a specific question.  

#### *Reviewers:*  
- GET /assigned-questions: View questions assigned for review.  
- POST /update-review-status: Approve or reject a question.  

### *User Management Endpoints (Admin)*  
- GET /users: View all users (educators and reviewers).  
- POST /update-user-role: Update a user's role or permissions.  

---

## Entity-Relationship Diagram (ERD)  
![ERD Diagram](erd.png)

## Data Flow Diagram (DFD)  
![DFD Diagram](dfd.png)  

---

## Final Summary  

The *Question Setting Platform* is a comprehensive solution for streamlining the creation and review of examination questions. It integrates role-specific functionalities for educators, reviewers, and administrators, ensuring an optimal user experience for all stakeholders.  

### *Key Highlights:*  
- Advanced tools for question creation and review.  
- Real-time updates for question approval processes.  
- Secure and scalable architecture using Node.js, React.js, and MongoDB.  
- Robust role-based access control with JWT.  

With its intuitive interface and efficient backend, the Question Setting Platform ensures a seamless flow of operations from question creation to final approval.  

---  

*Thank You!*  

This documentation provides a complete overview of the platform, including requirements, API endpoints, and system diagrams.
