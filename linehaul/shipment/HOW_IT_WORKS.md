# How it works?

The Shipment solution is a set of APIs that allows you to create, manage and track shipments. A shipment is a transportation/vehicle that will carry the consignment(s), that we book with a carrier company, and has price and capacity (loading unity type). Shipment can have more than one pick up and one drop off location and can carry multiple consignments.

The main entities of the Shipment solution are:

- **Shipment**: A transportation/vehicle that will carry the consignment(s), that we book with a carrier company, and has price and capacity (loading unity type). Shipment can have more than one pick up and one drop off location and can carry multiple consignments.
- **Consignable Unit**: A group of goods that will be transported together, with one sender and one receiver unit. It could be considered as Freight, Cargo or Load. Consignment(CSM) can consist of customer orders, or Handling Materials  or replenishment orders or any other type of goods to be transported. Every item within a CSM transported together, all of them are picked up from one location and dropped off at one location.
- **Consignment**: A group of goods that will be transported together, with one sender and one receiver unit. It could be considered as Freight, Cargo or Load. Consignment(CSM) can consist of customer orders, or Handling Materials  or replenishment orders or any other type of goods to be transported. Every item within a CSM transported together, all of them are picked up from one location and dropped off at one location.
- **Consignment Proposal**: A draft of the shipment you will create on your system. It is a proposal of the consignments that will be transported together in a shipment.
- **Consignment Proposal Item**: A draft of the consignment you will create on your system. It is a proposal of the consignable units that will be transported together in a consignment.
- **Consignment Proposal Item Rating**: A rating of the consignable units that will compose your consignment based on the pricing configured.
- **Consignment Proposal Item Rating Component**: A rating component of the consignable units that will compose your consignment based on the pricing configured.
- **Consignment Proposal Item Rating Component Value**: A rating component value of the consignable units that will compose your consignment based on the pricing configured.