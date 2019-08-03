# calculation-question/core Schema

```

```

| Abstract            | Extensible | Status       | Identifiable | Custom Properties | Additional Properties | Defined In                                                           |
| ------------------- | ---------- | ------------ | ------------ | ----------------- | --------------------- | -------------------------------------------------------------------- |
| Can be instantiated | No         | Experimental | No           | Forbidden         | Permitted             | [calculation-exercise.schema.json](calculation-exercise.schema.json) |

# calculation-question/core Properties

| Property                              | Type       | Required     | Nullable | Defined by                                 |
| ------------------------------------- | ---------- | ------------ | -------- | ------------------------------------------ |
| [calculations](#calculations)         | `object[]` | **Required** | No       | calculation-question/core (this schema)    |
| [shuffled](#shuffled)                 | `boolean`  | **Required** | No       | calculation-question/core (this schema)    |
| [task-description](#task-description) | `object[]` | **Required** | No       | calculation-question/core (this schema)    |
| [type](#type)                         | `enum`     | **Required** | No       | calculation-question/core (this schema)    |
| [with-oom](#with-oom)                 | `boolean`  | **Required** | No       | calculation-question/core (this schema)    |
| [with-units](#with-units)             | `boolean`  | **Required** | No       | calculation-question/core (this schema)    |
| `*`                                   | any        | Additional   | Yes      | this schema _allows_ additional properties |

## calculations

`calculations`

- is **required**
- type: `object[]`
- defined in this schema

### calculations Type

Array type: `object[]`

All items must be of the type: `object` with following properties:

| Property             | Type    | Required     |
| -------------------- | ------- | ------------ |
| `correct-points`     | integer | **Required** |
| `id`                 | string  | **Required** |
| `incorrect-points`   | integer | **Required** |
| `name`               | string  | **Required** |
| `number`             | string  | **Required** |
| `order-of-magnitude` | string  | **Required** |
| `units`              | array   | **Required** |

#### correct-points

`correct-points`

- is **required**
- type: `integer`

##### correct-points Type

`integer`

#### id

`id`

- is **required**
- type: `string`

##### id Type

`string`

#### incorrect-points

`incorrect-points`

- is **required**
- type: `integer`

##### incorrect-points Type

`integer`

#### name

`name`

- is **required**
- type: `string`

##### name Type

`string`

#### number

`number`

- is **required**
- type: `string`

##### number Type

`string`

#### order-of-magnitude

`order-of-magnitude`

- is **required**
- type: `string`

##### order-of-magnitude Type

`string`

#### units

`units`

- is **required**
- type: `object[]`

##### units Type

Array type: `object[]`

All items must be of the type: `object` with following properties:

| Property | Type   | Required     |
| -------- | ------ | ------------ |
| `expo`   | string | **Required** |
| `prefix` | string | **Required** |
| `unit`   | string | **Required** |

#### expo

`expo`

- is **required**
- type: `string`

##### expo Type

`string`

#### prefix

`prefix`

- is **required**
- type: `string`

##### prefix Type

`string`

#### unit

`unit`

- is **required**
- type: `string`

##### unit Type

`string`

## shuffled

`shuffled`

- is **required**
- type: `boolean`
- defined in this schema

### shuffled Type

`boolean`

## task-description

`task-description`

- is **required**
- type: `object[]`
- defined in this schema

### task-description Type

Array type: `object[]`

All items must be of the type: `object` with following properties:

| Property | Type | Required |
| -------- | ---- | -------- |


## type

`type`

- is **required**
- type: `enum`
- defined in this schema

The value of this property **must** be equal to one of the [known values below](#type-known-values).

### type Known Values

| Value         | Description |
| ------------- | ----------- |
| `calculation` |             |

## with-oom

`with-oom`

- is **required**
- type: `boolean`
- defined in this schema

### with-oom Type

`boolean`

## with-units

`with-units`

- is **required**
- type: `boolean`
- defined in this schema

### with-units Type

`boolean`
