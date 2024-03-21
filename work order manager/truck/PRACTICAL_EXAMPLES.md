# Practical Examples

## Example 1: Shipment of a single item

Let's say you have a single item to be transported from one location to another. You can create a shipment for this item. The shipment will have a sender and a receiver, and the item will be picked up from the sender's location and dropped off at the receiver's location.

### Request

```json
{
  "shipment": {
    "sender": {
      "name": "John Doe",
      "address": "123 Main St, Springfield, IL 62701"
    },
    "receiver": {
      "name": "Jane Doe",
      "address": "456 Elm St, Springfield, IL 62702"
    },
    "consignments": [
      {
        "sender": {
          "name": "John Doe",
          "address": "123 Main St, Springfield, IL 62701"
        },
        "receiver": {
          "name": "Jane Doe",
          "address": "456 Elm St, Springfield, IL 62702"
        },
        "items": [
          {
            "name": "Widget",
            "quantity": 1,
            "weight": 1.5,
            "volume": 0.5
          }
        ]
      }
    ]
  }
}
```

### Response

```json
{
  "shipment": {
    "id": "SHM.123",
    "status": "In Transit",
    "sender": {
      "name": "John Doe",
      "address": "123 Main St, Springfield, IL 62701"
    },
    "receiver": {
      "name": "Jane Doe",
      "address": "456 Elm St, Springfield, IL 62702"
    },
    "consignments": [
      {
        "id": "CON.456",
        "status": "In Transit",
        "sender": {
          "name": "John Doe",
          "address": "123 Main St, Springfield, IL 62701"
        },
        "receiver": {
          "name": "Jane Doe",
          "address": "456 Elm St, Springfield, IL 62702"
        },
        "items": [
          {
            "id": "ITM.789",
            "name": "Widget",
            "quantity": 1,
            "weight": 1.5,
            "volume": 0.5
          }
        ]
      }
    ]
  }
}
```

## Example 2: Shipment of multiple items

Let's say you have multiple items to be transported from one location to another. You can create a shipment for these items. The shipment will have a sender and a receiver, and the items will be picked up from the sender's location and dropped off at the receiver's location.

### Request

```json
{
  "shipment": {
    "sender": {
      "name": "John Doe",
      "address": "123 Main St, Springfield, IL 62701"
    },
    "receiver": {
      "name": "Jane Doe",
      "address": "456 Elm St, Springfield, IL 62702"
    },
    "consignments": [
      {
        "sender": {
          "name": "John Doe",
          "address": "123 Main St, Springfield, IL 62701"
        },
        "receiver": {
          "name": "Jane Doe",
          "address": "456 Elm St, Springfield, IL 62702"
        },
        "items": [
          {
            "name": "Widget",
            "quantity": 1,
            "weight": 1.5,
            "volume": 0.5
          },
          {
            "name": "Gadget",
            "quantity": 2,
            "weight": 2.5,
            "volume": 1.0
          }
        ]
      }
    ]
  }
}
```

### Response

```json
{
  "shipment": {
    "id": "SHM.123",
    "status": "In Transit",
    "sender": {
      "name": "John Doe",
      "address": "123 Main St, Springfield, IL 62701"
    },
    "receiver": {
      "name": "Jane Doe",
      "address": "456 Elm St, Springfield, IL 62702"
    },
    "consignments": [
      {
        "id": "CON.456",
        "status": "In Transit",
        "sender": {
          "name": "John Doe",
          "address": "123 Main St, Springfield, IL 62701"
        },
        "receiver": {
          "name": "Jane Doe",
          "address": "456 Elm St, Springfield, IL 62702"
        },
        "items": [
          {
            "id": "ITM.789",
            "name": "Widget",
            "quantity": 1,
            "weight": 1.5,
            "volume": 0.5
          },
          {
            "id": "ITM.101",
            "name": "Gadget",
            "quantity": 2,
            "weight": 2.5,
            "volume": 1.0
          }
        ]
      }
    ]
  }
}
```
