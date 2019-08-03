---
layout: default
---

# common/answer Schema

```

```

| Abstract            | Extensible | Status       | Identifiable | Custom Properties | Additional Properties | Defined In                               |
| ------------------- | ---------- | ------------ | ------------ | ----------------- | --------------------- | ---------------------------------------- |
| Can be instantiated | No         | Experimental | No           | Forbidden         | Permitted             | [answer.schema.json](answer.schema.json) |

# common/answer Properties

| Property            | Type      | Required     | Nullable | Defined by                                 |
| ------------------- | --------- | ------------ | -------- | ------------------------------------------ |
| [correct](#correct) | `boolean` | **Required** | No       | common/answer (this schema)                |
| [points](#points)   | `number`  | **Required** | No       | common/answer (this schema)                |
| [text](#text)       | `string`  | **Required** | No       | common/answer (this schema)                |
| `*`                 | any       | Additional   | Yes      | this schema _allows_ additional properties |

## correct

`correct`

- is **required**
- type: `boolean`
- defined in this schema

### correct Type

`boolean`

## points

`points`

- is **required**
- type: `number`
- defined in this schema

### points Type

`number`

## text

`text`

- is **required**
- type: `string`
- defined in this schema

### text Type

`string`
