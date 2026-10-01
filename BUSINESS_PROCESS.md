# Business Process

## Before vs. After

## Existing Manual Process

The original equipment-ordering process involved several disconnected
steps.

``` text
QuickBooks
    ↓
Export Excel
    ↓
Open Estimate
    ↓
Review Equipment
    ↓
Manually Enter / Adjust Quantities
    ↓
Create ICO Lines
    ↓
SharePoint Request
    ↓
Email Procurement
    ↓
Procurement Processing
    ↓
Separate Tracking
```

### Main problems

-   Manual data entry
-   Duplicate information
-   Multiple systems
-   Manual ICO creation
-   Email dependency
-   Limited order visibility
-   Difficult historical tracking
-   Additional effort for change orders

------------------------------------------------------------------------

## Proposed Process

``` text
Import Project Data
        ↓
Review Project
        ↓
Review Equipment
        ↓
Add / Adjust Equipment
        ↓
Separate Estimated & ICO Items
        ↓
Build Order Basket
        ↓
Review Request
        ↓
Finalize Order
        ↓
Generate Order #
        ↓
Procurement
        ↓
PO
        ↓
Ordered
        ↓
Received
        ↓
Historical Record
        ↓
Financial Reporting
```

------------------------------------------------------------------------

## Why the Workflow Changed

The application was designed to keep information together for the entire
lifecycle of an equipment request.

Instead of treating ordering as a single event, the system treats it as
a process:

``` text
Estimate
   ↓
Requirement
   ↓
Request
   ↓
Order
   ↓
PO
   ↓
Receiving
   ↓
Financial Record
```

This creates a continuous record from project estimate through
procurement.

------------------------------------------------------------------------

## Future Measurement

Once the application is used in a real workflow, the following
measurements can be captured:

-   Average time to prepare an order
-   Number of orders per month
-   Number of ICO items
-   Number of order revisions
-   Time spent by Procurement processing requests
-   Number of email-based follow-ups
-   Time from request to order
-   Time from order to received
-   Estimate value vs. ordered value

These measurements should be collected before claiming a specific
productivity improvement.
