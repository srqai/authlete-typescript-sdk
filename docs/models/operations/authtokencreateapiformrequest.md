# AuthTokenCreateApiFormRequest

## Example Usage

```typescript
import { AuthTokenCreateApiFormRequest } from "authlete-typescript-sdk/models/operations";

let value: AuthTokenCreateApiFormRequest = {
  serviceId: "<id>",
  apiServiceIdAuthTokenCreate: {
    grantType: "IMPLICIT",
    clientId: 62300,
  },
};
```

## Fields

| Field                                                                             | Type                                                                              | Required                                                                          | Description                                                                       |
| --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- |
| `serviceId`                                                                       | *string*                                                                          | :heavy_check_mark:                                                                | A service ID.                                                                     |
| `apiServiceIdAuthTokenCreate`                                                     | [models.ApiServiceIdAuthTokenCreate](../../models/apiserviceidauthtokencreate.md) | :heavy_check_mark:                                                                | N/A                                                                               |