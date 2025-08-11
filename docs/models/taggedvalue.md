# TaggedValue

An object containing taggedvalue data

## Example Usage

```typescript
import { TaggedValue } from "authlete-2/models";

let value: TaggedValue = {};
```

## Fields

| Field                  | Type                   | Required               | Description            |
| ---------------------- | ---------------------- | ---------------------- | ---------------------- |
| `tag`                  | *string*               | :heavy_minus_sign:     | The language tag part. |
| `value`                | *string*               | :heavy_minus_sign:     | The value part.        |