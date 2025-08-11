# AuthTokenUpdateApiFormRequest

## Example Usage

```typescript
import { AuthTokenUpdateApiFormRequest } from "authlete-2/models/operations";

let value: AuthTokenUpdateApiFormRequest = {
  serviceId: "<id>",
  apiServiceIdAuthTokenUpdate: {
    accessToken: "<value>",
  },
};
```

## Fields

| Field                                                                             | Type                                                                              | Required                                                                          | Description                                                                       |
| --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- |
| `serviceId`                                                                       | *string*                                                                          | :heavy_check_mark:                                                                | A service ID.                                                                     |
| `apiServiceIdAuthTokenUpdate`                                                     | [models.ApiServiceIdAuthTokenUpdate](../../models/apiserviceidauthtokenupdate.md) | :heavy_check_mark:                                                                | N/A                                                                               |