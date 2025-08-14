# AuthTokenRevokeApiFormRequest

## Example Usage

```typescript
import { AuthTokenRevokeApiFormRequest } from "authlete-typescript-sdk/models/operations";

let value: AuthTokenRevokeApiFormRequest = {
  serviceId: "<id>",
  tokenRevokeRequest: {},
};
```

## Fields

| Field                                                           | Type                                                            | Required                                                        | Description                                                     |
| --------------------------------------------------------------- | --------------------------------------------------------------- | --------------------------------------------------------------- | --------------------------------------------------------------- |
| `serviceId`                                                     | *string*                                                        | :heavy_check_mark:                                              | A service ID.                                                   |
| `tokenRevokeRequest`                                            | [models.TokenRevokeRequest](../../models/tokenrevokerequest.md) | :heavy_check_mark:                                              | N/A                                                             |