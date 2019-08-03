# learning-object-schema/exercise Schema

```

```

| Abstract            | Extensible | Status       | Identifiable | Custom Properties | Additional Properties | Defined In                                   |
| ------------------- | ---------- | ------------ | ------------ | ----------------- | --------------------- | -------------------------------------------- |
| Can be instantiated | No         | Experimental | No           | Forbidden         | Permitted             | [exercise.schema.json](exercise.schema.json) |

# learning-object-schema/exercise Properties

| Property      | Type     | Required     | Nullable | Defined by                                    |
| ------------- | -------- | ------------ | -------- | --------------------------------------------- |
| [core](#core) | `object` | **Required** | No       | learning-object-schema/exercise (this schema) |
| [type](#type) | `enum`   | **Required** | No       | learning-object-schema/exercise (this schema) |
| `*`           | any      | Additional   | Yes      | this schema _allows_ additional properties    |

## core

`core`

- is **required**
- type: `object`
- defined in this schema

### core Type

`object` with following properties:

| Property | Type | Required     |
| -------- | ---- | ------------ |
| `type`   |      | **Required** |

#### type

`type`

- is **required**
- type: `enum`

The value of this property **must** be equal to one of the [known values below](#core-known-values).

##### type Known Values

| Value                   | Description |
| ----------------------- | ----------- |
| `expression`            |             |
| `single-choice`         |             |
| `programming`           |             |
| `simple-text`           |             |
| `multistep-calculation` |             |
| `list`                  |             |
| `calculation`           |             |
| `multiple-choice`       |             |
| `sorting`               |             |

## type

`type`

- is **required**
- type: `enum`
- defined in this schema

The value of this property **must** be equal to one of the [known values below](#type-known-values).

### type Known Values

| Value      | Description |
| ---------- | ----------- |
| `exercise` |             |
