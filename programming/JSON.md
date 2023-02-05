# JSON

Filename extension: `.json`
Official website: [json.org](https://www.json.org/json-en.html)

## What is JSON

**JSON** (**JavaScript Object Notation**), is an open standard file format and data interchange format. It uses "human-readable" text to store and transmit data objects consisting of `attribute-value` pairs and arrays (or other serializable values). JSON is often used in web-applications.

## Syntax

The following example shows a JSON file that represents a description about a person:

```json
{
  "firstName": "John",
  "lastName": "Smith",
  "isAlive": true,
  "age": 27,
  "address": {
    "streetAddress": "21 2nd Street",
    "city": "New York",
    "state": "NY",
    "postalCode": "10021-3100"
  },
  "phoneNumbers": [
    {
      "type": "home",
      "number": "212 555-1234"
    },
    {
      "type": "office",
      "number": "646 555-4567"
    }
  ],
  "children": [
      "Catherine",
      "Thomas",
      "Trevor"
  ],
  "spouse": null
}
```

## Data-Types

JSON's basic data types are:

- number 
- string
- boolean
- array
- object
- null

---

#json 
