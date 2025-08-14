# AuthTokenApiFormRequest

## Example Usage

```typescript
import { AuthTokenApiFormRequest } from "authlete-typescript-sdk/models/operations";

let value: AuthTokenApiFormRequest = {
  serviceId: "<id>",
  tokenRequest: {},
};
```

## Fields

| Field                                               | Type                                                | Required                                            | Description                                         |
| --------------------------------------------------- | --------------------------------------------------- | --------------------------------------------------- | --------------------------------------------------- |
| `serviceId`                                         | *string*                                            | :heavy_check_mark:                                  | A service ID.                                       |
| `tokenRequest`                                      | [models.TokenRequest](../../models/tokenrequest.md) | :heavy_check_mark:                                  | N/A                                                 |