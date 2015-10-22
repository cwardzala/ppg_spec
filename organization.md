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
    "ils_enabled": false
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

### 2.3 `ils_enabled` member
The `ils_enabled` member is a __Boolean__ that identifies if the Organization has ILS grid ordering enabled. If this value is _false_ then it overrides any `ils_enabled` value for the [Customer](customer.md).
