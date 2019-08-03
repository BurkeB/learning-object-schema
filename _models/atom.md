---
layout: default
---
# Schema

```

```
{{ include lom_preview.html content="abc"}}

| Abstract            | Extensible | Status       | Identifiable | Custom Properties | Additional Properties |
| ------------------- | ---------- | ------------ | ------------ | ----------------- | --------------------- |
| Can be instantiated | No         | Experimental | No           | Forbidden         | Permitted             |

# Properties

| Property              | Type     | Required     | Nullable | Defined by                                 |
| --------------------- | -------- | ------------ | -------- | ------------------------------------------ |
| [core](#core)         | `object` | **Required** | No       | (this schema)                              |
| [id](#id)             | `string` | **Required** | No       | (this schema)                              |
| [metadata](#metadata) | `object` | Optional     | No       | (this schema)                              |
| [title](#title)       | `string` | **Required** | No       | (this schema)                              |
| [type](#type)         | `enum`   | **Required** | No       | (this schema)                              |
| `*`                   | any      | Additional   | Yes      | this schema _allows_ additional properties |

## core

### atom/core

`core`

- is **required**
- type: `object`
- defined in this schema

### core Type

`object` with following properties:

| Property | Type  | Required |
| -------- | ----- | -------- |
| `tags`   | array | Optional |

#### tags

`tags`

- is optional
- type: `string[]`

##### tags Type

Array type: `string[]`

All items must be of the type: `string`

## id

`id`

- is **required**
- type: `string`
- defined in this schema

### id Type

`string`

## metadata

### atom/metadata

`metadata`

- is optional
- type: `object`
- defined in this schema

### metadata Type

`object` with following properties:

| Property | Type  | Required |
| -------- | ----- | -------- |
| `tags`   | array | Optional |

#### tags

`tags`

- is optional
- type: `string[]`

##### tags Type

Array type: `string[]`

All items must be of the type: `string`

## title

`title`

- is **required**
- type: `string`
- defined in this schema

### title Type

`string`

## type

`type`

- is **required**
- type: `enum`
- defined in this schema

The value of this property **must** be equal to one of the [known values below](#type-known-values).

### type Known Values

| Value      | Description |
| ---------- | ----------- |
| `video`    |             |
| `section`  |             |
| `exercise` |             |
| `page`     |             |
