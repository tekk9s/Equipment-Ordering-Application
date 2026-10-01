# Features

## Project Management

-   Create/import projects
-   Assign projects to users
-   Distinguish Main Projects and Change Orders
-   Associate Change Orders with Main Projects
-   Manage project information

## Equipment Management

-   View equipment requirements
-   Track estimated equipment
-   Add ICO equipment
-   Edit quantities
-   Remove equipment
-   Preserve historical context
-   Search approved/available price-book items where applicable

## Ordering

-   Add equipment to an order basket
-   Review order contents
-   Edit quantities before finalization
-   Remove order lines
-   Finalize an order
-   Generate Order Number
-   Maintain order history
-   Support revisions

## Procurement

-   Procurement inbox
-   Search by Order Number
-   View requested orders
-   Update order status
-   Record PO numbers
-   Record receiving information
-   Record received dates
-   Manage procurement workflow

## Notifications

The application was designed to support notifications around important
procurement status changes.

Examples include:

``` text
Requested → Ordered
Ordered → Received
```

The exact notification implementation will continue to evolve during
development.

## User Management

Roles include:

-   Master User
-   Project Manager
-   Procurement Manager
-   Site Lead
-   View Only
-   Operation Manager

Permissions determine what users can view and modify.

## Financial Reporting

The Operation Manager's Financial Report is intended to provide:

-   Main Project selection
-   Estimate value
-   Ordered value
-   Difference between estimate and ordered value
-   Related Change Order compilation
-   Individual Change Order review

## Price Book / ICO Workflow

The application includes a concept for adding ICO items through a
controlled price-book workflow.

The intended process includes:

``` text
Search Price Book
      ↓
Select Item
      ↓
Enter Quantity
      ↓
Add as ICO
```

New items can be added to the price book with relevant information such
as:

-   Brand
-   Part Number
-   Description
-   Optional Unit Price

## Revision & History

The application is designed to preserve historical information rather
than simply overwriting records.

This includes:

-   Order history
-   Equipment changes
-   Revisions
-   Procurement status history
-   Receiving information
