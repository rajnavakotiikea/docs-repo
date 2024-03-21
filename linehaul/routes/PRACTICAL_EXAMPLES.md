# Practical Examples

## Example 1: Routes of a single item

Let's say you have a single item to be transported from one location to another. You can create a route for this item. The route will have a sender and a receiver, and the item will be picked up from the sender's location and dropped off at the receiver's location.

### Request

```json
{
  "route": {
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
}
```

### Response

```json
{
  "route": {
    "id": "RT.123",
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
}
```

## Example 2: Routes of multiple items

Let's say you have multiple items to be transported from one location to another. You can create a route for each item and group them together in a shipment. The route will have a sender and a receiver, and the items will be picked up from the sender's location and dropped off at the receiver's location.

### Request

```json
{
  "route": {
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
}
```

### Response

```json
{
  "route": {
    "id": "RT.123",
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
}
```