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

## Arrays of String in YAML

Strings contain a group of characters. It is a scalar type in yaml.

Keys in the string array are optional in YAML. Here is an example of an array of strings with keys.

```bash
    numbers: [  one,  two,  three,  four]
```

Arrays of strings without keys:

```bash
[
  one,
  two,
  three,
  four
]
```

## Arrays of Numbers

Integers

```bash
    numbers: [
  1,
  2,
  3,
  4
]
```

Floats:

```bash
    floatvalues: [
  1.3,
  2.2,
  3,
  4
]
```

## Yaml objects with arrays

The object contains key and value pairs. Value can be scalar or an array of scalar items.

```bash
author: Franc
database:
  driver: com.mysql.jdbc.Driver
  port: 3306
  dbname: students
  username: root
  password: root
support:
  - mysql
  - MongoDB
  - Postgres
```

## Dictionary in yaml example

The dictionary contains keys and values

Yaml Dictionary Two Types:

1. Flow mapping
2. Block mapping

### Flow Mapping

- key and value pairs are separated by a comma

- Entire pairs are enclosed in `{}`

- Syntax:

```bash
  # dictionary
mysqldatabase: {
    hostname: localhost,
    port: 3012, username:root,
    password: root
}
```

### Block Mapping

- Key and value pair are represented using colon `:`

```bash
# dictionary
  mysqldatabase:
    hostname: localhost
    port: 3012
    username: root
    password: root
```

Equivalent json:

```bash
{
  "mysqldatabase": {
    "hostname": "localhost",
    "port": 3012,
    "username": "root",
    "password": "root"
  }
}

```

## Empty Dictionary

```bash
employee: {}
```

OR

```bash
employee: null
```

## Empty Array

```bash
myvalue:""
```

OR

```bash
myvalue:[]
```
