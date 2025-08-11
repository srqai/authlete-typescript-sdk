# AuthTokenRevokeApiFormRequest

## Example Usage

```typescript
import { AuthTokenRevokeApiFormRequest } from "authlete-2/models/operations";

let value: AuthTokenRevokeApiFormRequest = {
  serviceId: "<id>",
  apiServiceIdAuthTokenRevoke: {},
};
```

## Fields

| Field                                                                             | Type                                                                              | Required                                                                          | Description                                                                       |
| --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- |
| `serviceId`                                                                       | *string*                                                                          | :heavy_check_mark:                                                                | A service ID.                                                                     |
| `apiServiceIdAuthTokenRevoke`                                                     | [models.ApiServiceIdAuthTokenRevoke](../../models/apiserviceidauthtokenrevoke.md) | :heavy_check_mark:                                                                | N/A                                                                               |