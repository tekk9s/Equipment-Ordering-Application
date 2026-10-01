# Development Log

## Equipment Ordering Application

This document records the development of the application from the
original problem through the current development stage.

------------------------------------------------------------------------

## Phase 1 --- Identifying the Problem

### Original situation

The equipment-ordering process was largely manual.

The process involved:

**QuickBooks → Excel → manual equipment selection → ICO lines →
SharePoint request → Procurement email**

The problem was not simply that one step was slow. Information had to be
repeatedly transferred between different systems.

### Initial project idea

The first concept was referred to as **Job Ordering Tracker**.

The purpose was to create an application that could:

-   Import project information.
-   Display equipment requirements.
-   Allow users to identify what needed to be ordered.
-   Handle additional/ICO equipment.
-   Create a procurement request.
-   Track the request after submission.

The project later evolved into **Equipment Ordering**.

------------------------------------------------------------------------

## Phase 2 --- Importing Project Data

A major early requirement was importing existing project information
instead of manually rebuilding project records.

The application needed to work with existing QuickBooks/Excel exports.

### Important discovery

The QuickBooks export structure did not initially match the expected
column headers.

The Item and Qty information was located in specific spreadsheet columns
rather than using the expected headers.

This became an early example of an important development lesson:

> Real-world data rarely arrives in the perfectly structured format
> expected by an application.

The import process therefore had to be designed around the actual export
format.

------------------------------------------------------------------------

## Phase 3 --- Project and Change Order Structure

The application needed to distinguish between:

-   Main Projects
-   Change Orders

A Change Order could not exist independently when it represented
additional scope for an existing project.

The system therefore introduced a relationship:

``` text
Main Project
   |
   +--- Change Order
   +--- Change Order
   +--- Change Order
```

This relationship later became important for financial reporting.

------------------------------------------------------------------------

## Phase 4 --- Estimated vs. ICO Equipment

One of the most important business rules developed during the project
was the separation of estimated equipment and ICO equipment.

Example:

``` text
Original estimate:
5 readers

Actual requirement:
6 readers
```

The system should not simply change the estimate to 6.

Instead:

``` text
5 Readers — Estimated
1 Reader  — ICO
```

This preserves the original estimate and makes the additional
requirement visible.

This decision became important for:

-   Ordering
-   Change tracking
-   Financial reporting
-   Historical accuracy

------------------------------------------------------------------------

## Phase 5 --- Equipment Ordering Workflow

The original concept evolved toward a cart/order-basket workflow.

Instead of immediately submitting each equipment line, the user can
build a request, review it, make changes, and then finalize it.

The workflow became:

``` text
Equipment
   ↓
Add to Order
   ↓
Order Basket
   ↓
Review / Edit
   ↓
Finalize
   ↓
Order Number
   ↓
Procurement
```

Requirements added during this phase included:

-   Edit quantities
-   Remove lines
-   Add ICO items
-   Review before finalizing
-   Preserve order history
-   Generate an Order Number

------------------------------------------------------------------------

## Phase 6 --- Procurement Workflow

The application was expanded beyond simply creating requests.

Procurement needed its own workflow.

The system was designed around statuses such as:

``` text
Requested
    ↓
Ordered
    ↓
Received
```

Additional requirements included:

-   PO tracking
-   Order number search
-   Receiving dates
-   Procurement editing permissions
-   Notifications
-   Order grouping
-   Order history

The goal was to prevent the system from becoming another request form
that still required separate email communication.

------------------------------------------------------------------------

## Phase 7 --- User Roles

As the application grew, it became clear that different users needed
different permissions.

Roles introduced during development included:

-   Master User
-   Project Manager
-   Procurement Manager
-   Site Lead
-   View Only
-   Operation Manager

The application therefore evolved from a simple ordering tool into a
small internal business-management system.

------------------------------------------------------------------------

## Phase 8 --- Operation Manager & Financial Reporting

A new requirement introduced the **Operation Manager** role.

The Operation Manager needed broad visibility into operations and a
dedicated **Financial Report** area.

The financial report is intended to allow the user to:

1.  Select a Main Project.
2.  View the original estimate value.
3.  View the value of ordered equipment.
4.  Compare estimate vs. ordered value.
5.  Compile related Change Orders into the Main Project view.
6.  Review individual Change Orders separately.

This feature connects procurement data with project financial
visibility.

------------------------------------------------------------------------

## Phase 9 --- Revision & History

The project also introduced the need to preserve history.

Instead of simply overwriting information, the application needs to
maintain a record of changes where appropriate.

Examples include:

-   Order revisions
-   Equipment changes
-   Original vs. additional equipment
-   Order history
-   Receiving history

This was an important shift from building a simple form to building a
system that needs historical traceability.

------------------------------------------------------------------------

## Phase 10 --- Current Development

The application remains under active development.

Future log entries will document:

-   New features
-   Bugs
-   Technical challenges
-   Database changes
-   API work
-   UI improvements
-   Testing
-   Screenshots
-   Deployment
-   User feedback
-   Measured business impact

------------------------------------------------------------------------

## Development Philosophy

A recurring theme throughout development has been:

> Build around the real business process, not around an idealized
> example.

Requirements changed as the workflow was examined more closely.

That iterative process is itself an important part of the project.
