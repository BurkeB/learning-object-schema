# programming-question/core Schema

```

```

| Abstract            | Extensible | Status       | Identifiable | Custom Properties | Additional Properties | Defined In                                                           |
| ------------------- | ---------- | ------------ | ------------ | ----------------- | --------------------- | -------------------------------------------------------------------- |
| Can be instantiated | No         | Experimental | No           | Forbidden         | Permitted             | [programming-exercise.schema.json](programming-exercise.schema.json) |

# programming-question/core Properties

| Property                        | Type       | Required     | Nullable | Defined by                                 |
| ------------------------------- | ---------- | ------------ | -------- | ------------------------------------------ |
| [code-template](#code-template) | `string`   | Optional     | No       | programming-question/core (this schema)    |
| [language](#language)           | complex    | **Required** | No       | programming-question/core (this schema)    |
| [type](#type)                   | `enum`     | **Required** | No       | programming-question/core (this schema)    |
| [unit-tests](#unit-tests)       | `object[]` | **Required** | No       | programming-question/core (this schema)    |
| `*`                             | any        | Additional   | Yes      | this schema _allows_ additional properties |

## code-template

`code-template`

- is optional
- type: `string`
- defined in this schema

### code-template Type

`string`

## language

`language`

- is **required**
- type: complex
- defined in this schema

### language Type

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

| Value         | Description |
| ------------- | ----------- |
| `programming` |             |

## unit-tests

`unit-tests`

- is **required**
- type: `object[]`
- defined in this schema

### unit-tests Type

Array type: `object[]`

All items must be of the type: `object` with following properties:

| Property           | Type   | Required     |
| ------------------ | ------ | ------------ |
| `correct-points`   | number | **Required** |
| `id`               | string | **Required** |
| `incorrect-points` | number | **Required** |
| `testcode`         | string | **Required** |
| `title`            | string | **Required** |

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

#### testcode

`testcode`

- is **required**
- type: `string`

##### testcode Type

`string`

#### title

`title`

- is **required**
- type: `string`

##### title Type

`string`
