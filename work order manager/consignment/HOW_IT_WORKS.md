# How it works?

This consignment preparation solution was built keeping in mind pricing configurability and cost model extensibility at its core. The architecture has been built ground up keeping in mind that different consignment and consignment models may be needed to be supported depending on the company pricing strategy. Because of that, before ingesting your first Consignable Unit (see [current supported consignable units](#supported-consignable)), there is a small set of configurations that you need to perform, but don't worry, we provide [APIs](#api-page) for this.

The basic usage flow of the solution would comprehend:

1. Get your API credentials via Authentication enrollment process. See [Authentication Enrollment and Setup](#authentication-enrollment)
2. Onboard the suppliers (service providers) for which the consignment statements will be created. See [Onboarding Suppliers](#onboarding-suppliers)
3. Create the Rate Cards with the prices that will be used on the cost calculation. See [Cost Models and Rate Cards](#cost-models-and-rate-cards)
4. Grab the schema of the event/request payload you will send. See [Consignable Unit Schemas](#consignable-unit-schemas)
5. Start ingesting the consignable units events you want to consign. See [Consignable Units Ingestion](#consignable-unit-ingestion)
6. Perform adjustments on the Consignable Units, like re-rating by different criterias, if needed. See [Re-rating and Adjustments on Consignable Units](#making-adjustments)
7. Create a Consignment Proposal that will contain the consignable units from a specific supplier and a period in time. See [Managing Consignment Proposals](#consignment-proposals)
8. Update Consignment Proposal statuses to reflect the current state of that consignment process. See [Consignment Proposal management](#consignment-proposal-management)
9. Create a Consignment that will contain the consignable units from a specific supplier and a period in time. See [Managing Consignments](#consignments)
10. Update Consignment statuses to reflect the current state of that consignment process. See [Consignment management](#consignment-management)