# simpletext/core Schema

```

```

| Abstract            | Extensible | Status       | Identifiable | Custom Properties | Additional Properties | Defined In                                                           |
| ------------------- | ---------- | ------------ | ------------ | ----------------- | --------------------- | -------------------------------------------------------------------- |
| Can be instantiated | No         | Experimental | No           | Forbidden         | Permitted             | [simple-text-exercise.schema.json](simple-text-exercise.schema.json) |

# simpletext/core Properties

| Property              | Type      | Required     | Nullable | Defined by                                 |
| --------------------- | --------- | ------------ | -------- | ------------------------------------------ |
| [points](#points)     | `number`  | **Required** | No       | simpletext/core (this schema)              |
| [shuffled](#shuffled) | `boolean` | Optional     | No       | simpletext/core (this schema)              |
| [textsize](#textsize) | `object`  | **Required** | No       | simpletext/core (this schema)              |
| [type](#type)         | `enum`    | **Required** | No       | simpletext/core (this schema)              |
| [voting](#voting)     | `boolean` | Optional     | No       | simpletext/core (this schema)              |
| `*`                   | any       | Additional   | Yes      | this schema _allows_ additional properties |

## points

`points`

- is **required**
- type: `number`
- defined in this schema

### points Type

`number`

## shuffled

`shuffled`

- is optional
- type: `boolean`
- defined in this schema

### shuffled Type

`boolean`

## textsize

`textsize`

- is **required**
- type: `object`
- defined in this schema

### textsize Type

`object` with following properties:

| Property | Type    | Required     |
| -------- | ------- | ------------ |
| `max`    | integer | **Required** |
| `min`    | number  | **Required** |
| `unit`   |         | **Required** |

#### max

`max`

- is **required**
- type: `integer`

##### max Type

`integer`

- minimum value: `1`

#### min

`min`

- is **required**
- type: `number`

##### min Type

`number`

#### unit

`unit`

- is **required**
- type: `enum`

The value of this property **must** be equal to one of the [known values below](#textsize-known-values).

##### unit Known Values

| Value        | Description |
| ------------ | ----------- |
| `characters` |             |
| `words`      |             |

## type

`type`

- is **required**
- type: `enum`
- defined in this schema

The value of this property **must** be equal to one of the [known values below](#type-known-values).

### type Known Values

| Value         | Description |
| ------------- | ----------- |
| `simple-text` |             |

## voting

`voting`

- is optional
- type: `boolean`
- defined in this schema

### voting Type

`boolean`
