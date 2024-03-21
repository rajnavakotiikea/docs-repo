# How it works?

The routes solution is a set of APIs that allows you to create, manage and track routes. A route is a sequence of locations that a vehicle will follow to deliver a consignment. The main entities of the routes solution are:

- **Route**: A sequence of locations that a vehicle will follow to deliver a consignment. It should have a valid date range and linked to available transportation options (carrier, loading unit/trailer options, prices) for that specific route.
- **Route Proposal**: A draft of the route you will create on your system. It is a proposal of the locations that will be visited in a route.
- **Route Proposal Item**: A draft of the location you will create on your system. It is a proposal of the locations that will be visited in a route.
- **Route Proposal Item Rating**: A rating of the locations that will compose your route based on the pricing configured.
- **Route Proposal Item Rating Component**: A rating component of the locations that will compose your route based on the pricing configured.
- **Route Proposal Item Rating Component Value**: A rating component value of the locations that will compose your route based on the pricing configured.
- **Route Proposal Item Rating Component Value**: A rating component value of the locations that will compose your route based on the pricing configured.

The main operations that you can perform with the routes solution are:

- Create a route with multiple locations
- Track the status of the route
- Manage the prices associated with its cost calculations
  