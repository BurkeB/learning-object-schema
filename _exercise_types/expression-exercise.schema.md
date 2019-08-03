# expression-question/core Schema

```

```

| Abstract            | Extensible | Status       | Identifiable | Custom Properties | Additional Properties | Defined In                                                         |
| ------------------- | ---------- | ------------ | ------------ | ----------------- | --------------------- | ------------------------------------------------------------------ |
| Can be instantiated | No         | Experimental | No           | Forbidden         | Permitted             | [expression-exercise.schema.json](expression-exercise.schema.json) |

# expression-question/core Properties

| Property                      | Type       | Required     | Nullable | Defined by                                 |
| ----------------------------- | ---------- | ------------ | -------- | ------------------------------------------ |
| [expressions](#expressions)   | `object[]` | **Required** | No       | expression-question/core (this schema)     |
| [input-format](#input-format) | complex    | **Required** | No       | expression-question/core (this schema)     |
| [type](#type)                 | `enum`     | **Required** | No       | expression-question/core (this schema)     |
| `*`                           | any        | Additional   | Yes      | this schema _allows_ additional properties |

## expressions

`expressions`

- is **required**
- type: `object[]`
- defined in this schema

### expressions Type

Array type: `object[]`

All items must be of the type: `object` with following properties:

| Property           | Type   | Required     |
| ------------------ | ------ | ------------ |
| `correct-points`   | number | **Required** |
| `id`               | string | **Required** |
| `incorrect-points` | number | **Required** |
| `text`             | string | **Required** |

#### correct-points

`correct-points`

- is **required**
- type: `number`

##### correct-points Type

`number`

#### id

`id`

- is **required**
- type: `string`

##### id Type

`string`

#### incorrect-points

`incorrect-points`

- is **required**
- type: `number`

##### incorrect-points Type

`number`

#### text

`text`

- is **required**
- type: `string`

##### text Type

`string`

## input-format

`input-format`

- is **required**
- type: complex
- defined in this schema

### input-format Type

Unknown type ``.

```json
{
  "isrequired": true,
  "simpletype": "complex"
}
```

## type

`type`

- is **required**
- type: `enum`
- defined in this schema

The value of this property **must** be equal to one of the [known values below](#type-known-values).

### type Known Values

| Value        | Description |
| ------------ | ----------- |
| `expression` |             |
