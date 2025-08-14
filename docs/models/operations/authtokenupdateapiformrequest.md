# AuthTokenUpdateApiFormRequest

## Example Usage

```typescript
import { AuthTokenUpdateApiFormRequest } from "authlete-typescript-sdk/models/operations";

let value: AuthTokenUpdateApiFormRequest = {
  serviceId: "<id>",
  tokenUpdateRequest: {},
};
```

## Fields

| Field                                                           | Type                                                            | Required                                                        | Description                                                     |
| --------------------------------------------------------------- | --------------------------------------------------------------- | --------------------------------------------------------------- | --------------------------------------------------------------- |
| `serviceId`                                                     | *string*                                                        | :heavy_check_mark:                                              | A service ID.                                                   |
| `tokenUpdateRequest`                                            | [models.TokenUpdateRequest](../../models/tokenupdaterequest.md) | :heavy_check_mark:                                              | N/A                                                             |