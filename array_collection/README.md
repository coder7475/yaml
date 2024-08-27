# YAML DataTypes

**Types**:

- Array of Scalar Items
- Array of objects
- Nested Array
- String array
- Object with values as an arrays
- empty array and objects
- sequence of elements
- Dictionary of elements

## Array of Scalar Items

An array is a group of similar values with a single name. In YAML, an Array represents a single key mapped to multiple values. Each value starts with a hyphen - symbol followed by a space.

Syntax:

```bash
    key1:
        - value1
        - value2
        - value3
        - value4
        - value5
```

You can rewrite this as in single line:

```bash
    key1: [value1,value2,value3,value4,value5]
```

Or multiple line:

```bash
    key1: [value1,value2
     value3,value4,value5]
```

The JSON Representation of it:

```bash
{
  "key1": [
    "value1",
    "value2",
    "value3",
    "value4",
    "value5"
  ]
}
```

## Array of Objects

Objects contain multiple key and value pairs. An array of objects contains an object list.

Example:

```bash
    one:
    - id: 1
        name: franc
    - id: 11
        name: Tom
```

Equivalent to:

```bash
    {
  "one": [
    {
      "id": 1,
      "name": "franc"
    },
    {
      "id": 11,
      "name": "Tom"
    }
  ]
}
```

## YAML nested arrays

Arrays of Arrays are also called multi-dimensional arrays or nested arrays.

Example of nested arrays using `indentation syntax` as below:

```bash
employees:
    -
        id: 213
        name: franc
        others:
            - { department: sales, did: 1}
            - { salary: 5000}
            - { address: USA, pincode: 97845 }

```

Equivalent to:

```bash
    {
  "employees": [
    {
      "id": 213,
      "name": "franc",
      "others": [
        {
          "department": "sales",
          "did": 1
        },
        {
          "Salary": 5000
        },
        {
          "address": "USA",
          "pincode": 97845
        }
      ]
    }
  ]
}
```
