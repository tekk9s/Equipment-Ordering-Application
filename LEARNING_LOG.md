# Learning Log

## Skills Developed Through the Equipment Ordering Application

This application is being used as a practical learning project. The goal
is to document not only what was built, but what was learned while
building it.

------------------------------------------------------------------------

## 1. Business Process Analysis

### What I learned

Before writing software, I needed to understand the existing process.

I learned to break a business workflow into:

-   Inputs
-   Users
-   Decisions
-   Data
-   Outputs
-   Bottlenecks
-   Repetitive tasks

### How I applied it

I mapped the existing equipment-ordering process and identified the
repeated movement of information between QuickBooks, Excel, SharePoint,
email, and Procurement.

------------------------------------------------------------------------

## 2. Requirements Gathering

### What I learned

Software requirements are not always known at the beginning.

As the application developed, new requirements appeared because the
initial design exposed additional business needs.

Examples:

-   ICO equipment
-   Change Order relationships
-   Order revisions
-   Procurement statuses
-   PO tracking
-   Receiving
-   Operation Manager
-   Financial reporting

### Key lesson

Building the first version helped reveal requirements that were
difficult to identify from the original workflow alone.

------------------------------------------------------------------------

## 3. JavaScript / TypeScript

### Concepts being learned

-   Variables
-   Functions
-   Objects
-   Arrays
-   Conditional logic
-   Types
-   Interfaces
-   Component logic
-   Error handling

### Practical application

Used to implement application behavior and business rules.

------------------------------------------------------------------------

## 4. React

### Concepts being learned

-   Components
-   Props
-   State
-   Forms
-   Event handling
-   Conditional rendering
-   Reusable UI elements
-   Tables and interactive controls

### Practical application

Used to create the application's interactive interface.

------------------------------------------------------------------------

## 5. Next.js

### Concepts being learned

-   Application structure
-   Routing
-   Pages
-   Server/client concepts
-   Application deployment concepts

------------------------------------------------------------------------

## 6. Node.js and npm

### Concepts being learned

-   Node.js runtime concepts
-   npm
-   Packages and dependencies
-   Development scripts
-   Build processes
-   Application tooling

### Practical lesson

I learned that modern web applications depend on an ecosystem of
packages and development tools rather than being a single standalone
program.

------------------------------------------------------------------------

## 7. APIs

### Concepts being learned

-   Client/server communication
-   Endpoints
-   Requests
-   Responses
-   JSON
-   Sending data
-   Receiving data
-   Error responses

### Practical application

APIs provide the communication layer between parts of the application
and its data/services.

------------------------------------------------------------------------

## 8. Databases

### Concepts being learned

-   Tables
-   Records
-   Primary identifiers
-   Relationships
-   Queries
-   Data persistence
-   Historical records

### Practical application

The application's projects, equipment, orders, users, and related
information need structured persistent storage.

------------------------------------------------------------------------

## 9. Cloudflare / D1

### Concepts being learned

-   Cloud-hosted application concepts
-   Database hosting
-   Cloudflare D1
-   Application deployment
-   Connecting application logic to hosted data

------------------------------------------------------------------------

## 10. Git & GitHub

### Concepts being learned

-   Repositories
-   Commits
-   Version history
-   Branches
-   Change tracking
-   Project documentation

The project itself will eventually serve as a documented example of
using GitHub to manage a software project.

------------------------------------------------------------------------

## 11. Authentication & Permissions

### Concepts being learned

-   User accounts
-   Roles
-   Permissions
-   Access control
-   Role-specific UI
-   Administrative controls

This became necessary because Project Managers, Procurement, Site Leads,
View Only users, and Operations have different responsibilities.

------------------------------------------------------------------------

## 12. Data Import

### Concepts being learned

-   Spreadsheet structure
-   Data mapping
-   Validation
-   Handling unexpected input formats
-   Import errors
-   Data normalization

### Practical lesson

Real business data needs to be handled defensively because export
formats are not always consistent with the application's ideal data
structure.

------------------------------------------------------------------------

## 13. Debugging

Debugging became one of the most important practical skills.

The development process involved identifying:

1.  What the application was expected to do.
2.  What it actually did.
3.  Where the behavior differed.
4.  Why the difference occurred.
5.  How to fix it.
6.  Whether the fix caused another problem.

This is different from simply writing new features.

------------------------------------------------------------------------

## 14. UI / UX Design

I learned to think about:

-   How users navigate the application
-   Reducing unnecessary clicks
-   Making information visible
-   Avoiding clutter
-   Tables and filtering
-   Clear status indicators
-   Role-specific navigation
-   Reviewing information before committing an action

------------------------------------------------------------------------

## 15. AI-Assisted Development

AI was used throughout development as a programming and problem-solving
assistant.

The workflow was:

``` text
Business requirement
       ↓
Explain requirement to AI
       ↓
Generate / modify implementation
       ↓
Run application
       ↓
Test
       ↓
Identify problem
       ↓
Explain problem
       ↓
Refine implementation
       ↓
Test again
```

The important skill developed was not simply generating code.

It was learning how to:

-   Describe a problem clearly
-   Break requirements into smaller tasks
-   Review generated code
-   Test functionality
-   Identify incorrect assumptions
-   Provide useful debugging information
-   Iterate toward the required behavior

------------------------------------------------------------------------

## 16. Most Important Overall Skill

The project combines **business knowledge with technology**.

I started with a real operational problem rather than a programming
exercise.

The development process required understanding:

**Business → Data → Workflow → Software → Testing → Improvement**

That combination is one of the main skills this project is intended to
demonstrate.
