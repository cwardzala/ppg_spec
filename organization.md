# Organization

## 1 Usage Examples
This section is non-normative.

This section shows how developers can make use of the features of this specification.

### 1.1 Example JSON

```json
{
    "id": "01fc7fce-bf78-4b50-903a-fb3b760f5b30",
    "name": {
        "long": "Cuyahoga County Public Library",
        "short": "CCPL"
    },
    "currency": "USD",
    "ils_enabled": false,
    "price_contracts": {
        "playaway_light": 0.25,
        "playaway_view": 0.05,
        "playaway_bookpacks": 0.05,
        "accessory": 0.25,
        "service": 0.25,
        "recorded_books": 0.05
    }
}
```

## 2 Organization and its members

### 2.1 `id` member
The `id` member is a __String__ [Universally unique identifier](https://en.wikipedia.org/wiki/Universally_unique_identifier) (UUID). Meant to represent a canonical ID for the Organization.

### 2.2 `name` member
The `name` member is an __Object__ that represents the Organization's naming information.

#### 2.2.1 `long` member
The `long` member represents the full name of the Organization.

#### 2.2.2 `short` member
The `long` member represents the short or abbreviated name of the Organization. This is provided for use when the full (long) name is not appropriate.

### 2.3 `currency` member
The `currency` member is a __String__ that represents the [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) alphabetic code for the Organization's default currency.

### 2.4 `ils_enabled` member
The `ils_enabled` member is a __Boolean__ that identifies if the Organization has ILS grid ordering enabled. If this value is _false_ then it overrides any `ils_enabled` value for the [Customer](customer.md).

### 2.5 `price_contracts` member
The `price_contracts` member is an __Object__ of _key:value_ pairs that identify the price contract discounts for zero or more product types. Each _key_ is a [Product](product.md) `format` member value, and its _value_ is the discount amount as a decimal __Float__.
