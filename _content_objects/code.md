---
title: Code
name: code
layout: content_object
---
# Code

## Properties

| Property              | Type     | Required     | Nullable | Defined by                                 |
| --------------------- | -------- | ------------ | -------- | ------------------------------------------ |
| [id](#id)         | `string` | **Required** | No       | (this schema)                              |
| [code](#code)         | `string` | **Required** | No       | (this schema)                              |
| [type](#type)         | `enum` (EDN: key / JS: string)   | **Required** | No       | (this schema)                              |
| [language](#language)         | `enum` (EDN: key / JS: string)   | **Required** | No       | (this schema)                              |
| `*`                   | any      | Additional   | Yes      | this schema _allows_ additional properties |


{{ site.models | where: "name", "ce-id" | first }}


### code

- is **required**
- type: `string`
- The code that is showed in the initial state.

### type

- is **required**
- type: enum
  - json-type: `string` -> `"code"`
  - edn-type: `key` -> `:code`

### language

- Programming Language of the given code.
- is **required**
- type: enum
  - json-type: `string`
  - edn-type: `key`
- Enum Values:
  - python3
  - javascript
- More languages will be specified in the future.

## Example

{% capture example_ce %}
{:id "2019-08-05T10-31-41-ce55",
    :type :code,
    :language :python3,
    :code "print(\"Hello World\")"}
{% endcapture %}

{% include lom_preview.html content=example_ce preview_id="code_preview" %}
