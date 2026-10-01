Equipment Ordering Application

Project Overview

Status: In development
Project: Internal Equipment Ordering & Procurement Application
Organization: Bond Securcom
Developer: Jason Le

This project began as an attempt to improve a manual equipment-ordering
process used for security construction projects.

The original workflow relied on information being moved between
QuickBooks exports, Excel estimates, SharePoint requests, and email. The
application is being developed to bring those steps into one centralized
workflow.

Portfolio note: Company names, project information, pricing,
employee information, and other proprietary data should be replaced
with fictional/sample data before this project is published publicly.

1. The Business Problem

The original equipment-ordering process required a Project Manager or
Project Coordinator to manually:

Export project information from QuickBooks.

Open and review the project estimate in Excel.

Determine which equipment needed to be ordered.

Manually enter or modify quantities.

Create separate lines for ICO (In-Change-Order) equipment when
equipment was not part of the original estimate.

Submit a request through SharePoint.

Email Procurement to notify them of the request.

Track the order separately from the original estimate.

This created several problems:

Repetitive data entry

Multiple systems containing pieces of the same information

Additional work when change-order equipment was required

Limited visibility into order status

Difficulty tracking revisions

Procurement communication being split between SharePoint and email

Additional effort when reviewing project financial information

The goal of the application is to reduce this manual work and create a
single workflow for project equipment ordering.

2. The Proposed Solution

The Equipment Ordering application centralizes project equipment and
procurement activities.

High-level workflow

QuickBooks / Excel
        |
        v
   Project Import
        |
        v
   Equipment Review
      /      \
Estimated    ICO
Equipment   Equipment
      \      /
        v
   Order Basket
        |
        v
   Order Request
        |
        v
    Procurement
        |
        +----> PO
        |
        +----> Ordered
        |
        +----> Received
        |
        v
   Order History
        |
        v
Financial Reporting

3. Core Features

The application has been developed around the following requirements:

Project import from existing spreadsheet data

Project and equipment management

Estimated equipment tracking

ICO equipment tracking

Main Project / Change Order relationships

Equipment ordering basket

Order request workflow

Generated Order Numbers

Procurement management

PO tracking

Receiving status and dates

Order history

Order revisions

User roles and permissions

Procurement notifications

Operation Manager oversight

Financial reporting

Estimate value vs. ordered value

Change-order financial consolidation

4. User Roles

The system was designed around different responsibilities within the
business.

Master User

Administrative/developer-level access for managing the system and users.

Project Manager

Manages assigned projects, equipment requirements, orders, and
project-related information.

Procurement Manager

Reviews and processes equipment requests, manages orders and POs, and
records receiving information.

Site Lead

Can work with existing projects and access the information needed for
site coordination.

View Only

Provides access to information without operational editing permissions.

Operation Manager

Provides broader oversight of operations and includes a dedicated
Financial Report area.

5. Important Business Rules

Estimated vs. ICO Equipment

ICO means equipment that was not part of the original estimate.

For example:

Estimated:
5 x Reader

Additional requirement:
1 x Reader

The system should represent this as:

5 x Reader — Estimated
1 x Reader — ICO

rather than changing the original estimated quantity.

This preserves the distinction between original scope and additional
equipment.

Change Orders

A change order can be associated with a Main Project.

This allows the application to:

Track change-order equipment separately.

Relate it back to the main project.

Compile change orders into the main project's financial view.

Still allow individual change orders to be reviewed separately.

Replacement Equipment

When an existing equipment model is replaced, the original item should
remain historically traceable rather than simply being overwritten.

The replacement can be represented as a new ICO item when appropriate.

6. Development Approach

This project is being developed iteratively.

The process has generally followed:

Business problem
      ↓
Requirement
      ↓
Prototype
      ↓
Test
      ↓
Identify issue
      ↓
Refine requirement
      ↓
Implement
      ↓
Test again

AI has been used as a development assistant during implementation,
debugging, design exploration, and code generation. The business
requirements, workflow decisions, testing, and iterative direction come
from the project owner.

7. Technology & Learning

The project has also been used as a practical way to learn software
development.

Technologies and concepts being documented include:

JavaScript / TypeScript

React

Next.js

Node.js / npm tooling

APIs

JSON

Database concepts

Cloudflare

Cloudflare D1

Git

GitHub

Authentication and permissions

Role-based access

Frontend/backend communication

Data import

Application state

Forms and validation

Debugging

AI-assisted development

The exact technology stack will be updated as development continues.

8. Screenshots & Visual Documentation

Screenshots are an important part of this project documentation.

Planned visual documentation includes:

Original manual workflow

Application login

Dashboard

Project list

Project details

Equipment table

ICO equipment

Order basket

Order submission

Procurement dashboard

PO tracking

Receiving

Order history

User permissions

Financial Report

Before/after workflow diagram

All public screenshots should use fictional or sanitized information.

9. Project Status

The application is still in development.

This README is intended to evolve with the application. Development
decisions, challenges, new features, screenshots, and lessons learned
will be added as the project progresses.

10. Portfolio Goal

The purpose of documenting this project is not simply to demonstrate
that an application was built.

It demonstrates the ability to:

Identify a real business problem

Understand an existing workflow

Gather and translate requirements

Design a software solution

Work with structured data

Build and test application functionality

Debug problems

Improve a system based on user requirements

Learn new technologies through practical application

Use AI as a development tool while maintaining ownership of the
business solution
