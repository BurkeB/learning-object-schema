# Schema

```

```

| Abstract            | Extensible | Status       | Identifiable | Custom Properties | Additional Properties | Defined In                                                               |
| ------------------- | ---------- | ------------ | ------------ | ----------------- | --------------------- | ------------------------------------------------------------------------ |
| Can be instantiated | No         | Experimental | No           | Forbidden         | Permitted             | [single-choice-exercise.schema.json](single-choice-exercise.schema.json) |

# Properties

| Property              | Type       | Required     | Nullable | Defined by                                 |
| --------------------- | ---------- | ------------ | -------- | ------------------------------------------ |
| [answers](#answers)   | `object[]` | **Required** | No       | (this schema)                              |
| [shuffled](#shuffled) | `boolean`  | Optional     | No       | (this schema)                              |
| [type](#type)         | `enum`     | **Required** | No       | (this schema)                              |
| [voting](#voting)     | `boolean`  | Optional     | No       | (this schema)                              |
| `*`                   | any        | Additional   | Yes      | this schema _allows_ additional properties |

## answers

`answers`

- is **required**
- type: `object[]`
- defined in this schema

### answers Type

Array type: `object[]`

All items must be of the type: `object` with following properties:

| Property            | Type   | Required     |
| ------------------- | ------ | ------------ |
| `id`                | string | **Required** |
| `selected-points`   | number | **Required** |
| `text`              | string | **Required** |
| `unselected-points` | number | **Required** |

#### id

`id`

- is **required**
- type: `string`

##### id Type

`string`

#### selected-points

`selected-points`

- is **required**
- type: `number`

##### selected-points Type

`number`

#### text

`text`

- is **required**
- type: `string`

##### text Type

`string`

#### unselected-points

`unselected-points`

- is **required**
- type: `number`

##### unselected-points Type

`number`

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

| Value           | Description |
| --------------- | ----------- |
| `single-choice` |             |

## voting

`voting`

- is optional
- type: `boolean`
- defined in this schema

### voting Type

`boolean`
