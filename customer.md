# Customer

## 1 Usage Examples
This section is non-normative.

This section shows how developers can make use of the features of this specification.

### 1.1 Example JSON

```json
{
    "id": "cf230493-3c8c-459b-a99b-30b137b350cd",
    "name": {
        "given": "John",
        "middle": "B",
        "family": "Doe"
    },
    "email": "jdoe@findaway.com",
    "is_approved": true,
    "org_id": 1234,
    "ils_enabled": false,
    "default_bp_pkg": "portfolio"
}
```

## 2 Manifest and its members

### 2.1 `id` member
The `id` member is a __String__ [Universally unique identifier](https://en.wikipedia.org/wiki/Universally_unique_identifier) (UUID). Meant to represent a canonical ID for the customer.

### 2.2 `name` member
The `name` member is an __Object__ that represents the customer's naming information.

#### 2.2.1 `given` member
The `given` member is a __String__ that represents the customer's given/first name.

#### 2.2.2 `middle` member
The `middle` member is a __String__ that represents the customer's middle name or abbreviation.

#### 2.2.3 `last` member
The `family` member is a __String__ that represents the customer's family/last/surname name.

### 2.3 `email` member
The `email` member is a __String__ that represents the customer's email address.

### 2.4 `is_approved` member
The `is_approved` member is a __Boolean__ that identifies if the customer is approved to order.

### 2.4 `ord_id` member
The `org_id` member is a __String__ that represents the `id` of an associated `Organization`.

### 2.4 `ils_enabled` member
The `ils_enabled` member is a __Boolean__ that identifies if the customer has ILS grid ordering enabled.

