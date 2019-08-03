# multiple-choice/core Schema

```

```

| Abstract            | Extensible | Status       | Identifiable | Custom Properties | Additional Properties | Defined In                                                                   |
| ------------------- | ---------- | ------------ | ------------ | ----------------- | --------------------- | ---------------------------------------------------------------------------- |
| Can be instantiated | No         | Experimental | No           | Forbidden         | Permitted             | [multiple-choice-exercise.schema.json](multiple-choice-exercise.schema.json) |

# multiple-choice/core Properties

| Property              | Type       | Required     | Nullable | Defined by                                 |
| --------------------- | ---------- | ------------ | -------- | ------------------------------------------ |
| [answers](#answers)   | `object[]` | **Required** | No       | multiple-choice/core (this schema)         |
| [shuffled](#shuffled) | `boolean`  | Optional     | No       | multiple-choice/core (this schema)         |
| [type](#type)         | `enum`     | **Required** | No       | multiple-choice/core (this schema)         |
| [voting](#voting)     | `boolean`  | Optional     | No       | multiple-choice/core (this schema)         |
| `*`                   | any        | Additional   | Yes      | this schema _allows_ additional properties |

## answers

`answers`

- is **required**
- type: `object[]`
- defined in this schema

### answers Type

Array type: `object[]`

All items must be of the type: `object` with following properties:

| Property           | Type   | Required     |
| ------------------ | ------ | ------------ |
| `checked-points`   | number | **Required** |
| `text`             | string | **Required** |
| `unchecked-points` | number | **Required** |

#### checked-points

`checked-points`

- is **required**
- type: `number`

##### checked-points Type

`number`

#### text

`text`

- is **required**
- type: `string`

##### text Type

`string`

#### unchecked-points

`unchecked-points`

- is **required**
- type: `number`

##### unchecked-points Type

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

| Value             | Description |
| ----------------- | ----------- |
| `multiple-choice` |             |

## voting

`voting`

- is optional
- type: `boolean`
- defined in this schema

### voting Type

`boolean`
