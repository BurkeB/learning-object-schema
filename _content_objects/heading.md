---
title: Heading
name: heading
layout: content_object
---
# Heading

## Properties

| Property              | Type     | Required     | Nullable | Defined by                                 |
| --------------------- | -------- | ------------ | -------- | ------------------------------------------ |
| [id](#id)         | `string` | **Required** | No       | (this schema)                              |
| [value](#code)         | `string` | **Required** | No       | (this schema)                              |
| [type](#type)         | `enum` (EDN: key / JS: string)   | **Required** | No       | (this schema)                              |
| [section](#language)         | integer  | **Required** | No       | (this schema)                              |
| `*`                   | any      | Additional   | Yes      | this schema _allows_ additional properties |


{{ site.models | where: "name", "ce-id" | first }}


### value

- is **required**
- type: `string`
- The Text of the heading.

### type

- is **required**
- type: enum
  - json-type: `string` -> `"heading"`
  - edn-type: `key` -> `:heading`

### section

- Section defines the level of a Heading.
- is **required**
- type: integer
- values: 1 (inclusive) to 6 (inclusive)
- See [HTML Headings](https://www.w3.org/MarkUp/html3/headings.html)

## Example

{% capture example_ce %}
{:id "2019-08-05T10-54-05-ce66",
    :value "Example Headline",
    :type :heading,
    :section "2"}
{% endcapture %}

{% include lom_preview.html content=example_ce preview_id="heading_preview" %}
