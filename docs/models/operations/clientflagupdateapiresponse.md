# ClientFlagUpdateApiResponse

An object containing schema data

## Example Usage

```typescript
import { ClientFlagUpdateApiResponse } from "authlete-typescript-sdk/models/operations";

let value: ClientFlagUpdateApiResponse = {
  resultCode: "<value>",
  resultMessage: "<value>",
};
```

## Fields

| Field                                                      | Type                                                       | Required                                                   | Description                                                |
| ---------------------------------------------------------- | ---------------------------------------------------------- | ---------------------------------------------------------- | ---------------------------------------------------------- |
| `resultCode`                                               | *string*                                                   | :heavy_check_mark:                                         | The code which represents the result of the API call.      |
| `resultMessage`                                            | *string*                                                   | :heavy_check_mark:                                         | A short message which explains the result of the API call. |