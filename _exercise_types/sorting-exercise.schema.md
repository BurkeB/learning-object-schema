# sorting-question/core Schema

```

```

| Abstract            | Extensible | Status       | Identifiable | Custom Properties | Additional Properties | Defined In                                                   |
| ------------------- | ---------- | ------------ | ------------ | ----------------- | --------------------- | ------------------------------------------------------------ |
| Can be instantiated | No         | Experimental | No           | Forbidden         | Permitted             | [sorting-exercise.schema.json](sorting-exercise.schema.json) |

# sorting-question/core Properties

| Property              | Type       | Required     | Nullable | Defined by                                 |
| --------------------- | ---------- | ------------ | -------- | ------------------------------------------ |
| [answers](#answers)   | `object[]` | **Required** | No       | sorting-question/core (this schema)        |
| [shuffled](#shuffled) | `boolean`  | Optional     | No       | sorting-question/core (this schema)        |
| [type](#type)         | `enum`     | **Required** | No       | sorting-question/core (this schema)        |
| `*`                   | any        | Additional   | Yes      | this schema _allows_ additional properties |

## answers

`answers`

- is **required**
- type: `object[]`
- defined in this schema

### answers Type

Array type: `object[]`

All items must be of the type: `object` with following properties:

| Property  | Type    | Required     |
| --------- | ------- | ------------ |
| `correct` | boolean | **Required** |
| `points`  | number  | **Required** |
| `text`    | string  | **Required** |

#### correct

`correct`

- is **required**
- type: `boolean`

##### correct Type

`boolean`

#### points

`points`

- is **required**
- type: `number`

##### points Type

`number`

#### text

`text`

- is **required**
- type: `string`

##### text Type

`string`

## shuffled

`shuffled`

- is optional
- type: `boolean`
- defined in this schema

### shuffled Type

`boolean`

## type

`type`

- is **required**
- type: `enum`
- defined in this schema

The value of this property **must** be equal to one of the [known values below](#type-known-values).

### type Known Values

| Value     | Description |
| --------- | ----------- |
| `sorting` |             |
