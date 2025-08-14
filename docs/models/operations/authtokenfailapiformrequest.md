# AuthTokenFailApiFormRequest

## Example Usage

```typescript
import { AuthTokenFailApiFormRequest } from "authlete-typescript-sdk/models/operations";

let value: AuthTokenFailApiFormRequest = {
  serviceId: "<id>",
  tokenFailRequest: {},
};
```

## Fields

| Field                                                       | Type                                                        | Required                                                    | Description                                                 |
| ----------------------------------------------------------- | ----------------------------------------------------------- | ----------------------------------------------------------- | ----------------------------------------------------------- |
| `serviceId`                                                 | *string*                                                    | :heavy_check_mark:                                          | A service ID.                                               |
| `tokenFailRequest`                                          | [models.TokenFailRequest](../../models/tokenfailrequest.md) | :heavy_check_mark:                                          | N/A                                                         |