---
title: HTML
name: html
layout: content_object
---
# HTML

## Properties

| Property              | Type     | Required     | Nullable | Defined by                                 |
| --------------------- | -------- | ------------ | -------- | ------------------------------------------ |
| [id](#id)         | `string` | **Required** | No       | (this schema)                              |
| [value](#code)         | `string` | **Required** | No       | (this schema)                              |
| [type](#type)         | `enum` (EDN: key / JS: string)   | **Required** | No       | (this schema)                              |
| `*`                   | any      | Additional   | Yes      | this schema _allows_ additional properties |


{{ site.models | where: "name", "ce-id" | first }}


### value

- is **required**
- type: `string`
- The HTML Text.

### type

- is **required**
- type: enum
  - json-type: `string` -> `"html"`
  - edn-type: `key` -> `:html`

## Example

{% capture example_ce %}
{:id "2019-08-05T11-22-14-ce75",
  :value "<b>Test</b>",
  :type :html}
{% endcapture %}

{% include lom_preview.html content=example_ce preview_id="html_preview" %}
