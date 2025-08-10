# InfoApiResponse

## Example Usage

```typescript
import { InfoApiResponse } from "authlete-typescript-sdk/models/operations";

let value: InfoApiResponse = {
  version: "<value>",
  features: [
    "<value 1>",
  ],
};
```

## Fields

| Field                                  | Type                                   | Required                               | Description                            |
| -------------------------------------- | -------------------------------------- | -------------------------------------- | -------------------------------------- |
| `version`                              | *string*                               | :heavy_check_mark:                     | The server version.                    |
| `features`                             | *string*[]                             | :heavy_check_mark:                     | the features that the server supports. |