# AuthTokenFailApiFormRequest

## Example Usage

```typescript
import { AuthTokenFailApiFormRequest } from "authlete-2/models/operations";

let value: AuthTokenFailApiFormRequest = {
  serviceId: "<id>",
  apiServiceIdAuthTokenFail: {
    ticket: "<value>",
    reason: "INVALID_TARGET",
  },
};
```

## Fields

| Field                                                                         | Type                                                                          | Required                                                                      | Description                                                                   |
| ----------------------------------------------------------------------------- | ----------------------------------------------------------------------------- | ----------------------------------------------------------------------------- | ----------------------------------------------------------------------------- |
| `serviceId`                                                                   | *string*                                                                      | :heavy_check_mark:                                                            | A service ID.                                                                 |
| `apiServiceIdAuthTokenFail`                                                   | [models.ApiServiceIdAuthTokenFail](../../models/apiserviceidauthtokenfail.md) | :heavy_check_mark:                                                            | N/A                                                                           |