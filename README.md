# Mini-Upwork — Freelance Marketplace Platform

**A database course project for a freelance marketplace platform connecting clients and freelancers.**

## 1. Project Overview

Mini-Upwork is a web-based freelance marketplace that connects clients who need services with freelancers who provide them.

The platform supports the entire project lifecycle, including job posting, proposal submission, freelancer selection, contract management, milestone tracking, payment processing, and user reviews.

The primary focus of this project is relational database analysis, design, implementation, normalization, and transaction integrity.

## 2. Project Objectives

- Analyze business requirements and define business rules.
- Design a comprehensive ER/EER conceptual data model.
- Convert the conceptual model into a relational database schema.
- Apply database normalization up to 3NF/BCNF.
- Implement database tables, constraints, relationships, and sample data.
- Develop complex SQL queries, triggers, and views.
- Build a web application connected to the database.
- Ensure data consistency for projects, milestones, payments, and reviews.

## 3. Technology Stack

| Component | Technology |
|---|---|
| Backend | Python 3, Flask |
| Frontend | HTML5, CSS3, JavaScript |
| Database | Microsoft SQL Server |
| Database connectivity | pyodbc |
| API architecture | REST API |
| Version control | Git, GitHub |
| Database modeling | ER/EER diagrams |

## 4. User Roles

### Client
- Register and manage an account.
- Create and manage job postings.
- Review proposals and select freelancers.
- Create contracts and define project milestones.
- Track project progress and approve deliverables.
- Monitor payments and review freelancers.

### Freelancer
- Manage profile, skills, and work experience.
- Search and filter job postings.
- Submit proposals and quotations.
- Manage accepted projects and milestones.
- Submit deliverables for approval.
- Track payment status and review clients.

### Administrator
- Manage user accounts and job postings.
- Monitor projects and transactions.
- Handle disputes and reported content.
- Review platform activity and statistics.

## 5. Core Functional Modules

1. User authentication and role management.
2. Freelancer profiles and skills.
3. Job posting and search.
4. Proposal and application management.
5. Project and contract management.
6. Milestone and deadline tracking.
7. Payment and platform fee management.
8. Two-way user reviews.
9. Dispute management.
10. Administrative reports and statistics.

## 6. Database Design

### 6.1 Conceptual Design — ER/EER

The conceptual design follows these seven steps:

1. Identify entity types and distinguish entities from attributes.
2. Identify relationship types.
3. Assign attributes to entities and relationships.
4. Define attribute value domains.
5. Identify key attributes.
6. Specify relationship cardinalities.
7. Design specialization/generalization hierarchies and participation constraints where applicable.

Deliverables:
- Problem statement and business rules.
- Complete ER/EER diagram.
- Entity and relationship descriptions.
- Attribute, key, cardinality, and constraint definitions.

### 6.2 Logical Design and Normalization

- Map the ER/EER model to relational tables.
- Define primary keys and foreign keys.
- Identify functional dependencies.
- Normalize relations to 3NF/BCNF.
- Explain decomposition and relevant integrity constraints.

### 6.3 Physical Implementation

- SQL DDL scripts for schema creation.
- SQL DML scripts for sample data.
- At least 10 complex SQL queries.
- Trigger/view deliverables according to the course requirements.
- Appropriate indexes and integrity constraints.
- Database testing and validation.

## 7. Main Database Challenges

### Multi-party Transactions
Represent clients, freelancers, platform fees, and payment transactions while maintaining consistent financial records and transaction statuses.

### Project Milestones
Track milestone deadlines, allocated budgets, deliverables, approval statuses, and payment conditions.

### User Reviews
Store reviews and calculate aggregate ratings from valid review records while preventing duplicate reviews for the same review event.

### Data Integrity
Use primary keys, foreign keys, unique constraints, check constraints, and database transactions to preserve data consistency.

## 8. Proposed Database Entities

The initial entity list includes:

- Users
- Roles
- FreelancerProfiles
- Skills
- FreelancerSkills
- Jobs
- Proposals
- Projects
- Contracts
- Milestones
- Deliverables
- Payments
- Transactions
- Reviews
- Disputes

The final entities, attributes, relationships, and constraints will be determined during the requirements analysis and ER/EER design phases.

## 9. Project Structure

```text
Mini-Upwork/
├── README.md
├── docs/
│   ├── requirements.md
│   ├── business-rules.md
│   ├── database-design.md
│   ├── normalization.md
│   └── diagrams/
├── database/
│   ├── schema.sql
│   ├── seed.sql
│   ├── queries.sql
│   ├── triggers.sql
│   └── views.sql
├── src/
│   ├── backend/
│   │   ├── app.py
│   │   ├── config.py
│   │   ├── db.py
│   │   ├── routes/
│   │   └── services/
│   └── frontend/
│       ├── index.html
│       ├── css/
│       └── js/
