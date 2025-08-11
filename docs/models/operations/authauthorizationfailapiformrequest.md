# AuthAuthorizationFailApiFormRequest

## Example Usage

```typescript
import { AuthAuthorizationFailApiFormRequest } from "authlete-typescript-sdk/models/operations";

let value: AuthAuthorizationFailApiFormRequest = {
  serviceId: "<id>",
  apiServiceIdAuthAuthorizationFail: {
    ticket: "<value>",
    reason: "SERVER_ERROR",
  },
};
```

## Fields

| Field                                                                                         | Type                                                                                          | Required                                                                                      | Description                                                                                   |
| --------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- |
| `serviceId`                                                                                   | *string*                                                                                      | :heavy_check_mark:                                                                            | A service ID.                                                                                 |
| `apiServiceIdAuthAuthorizationFail`                                                           | [models.ApiServiceIdAuthAuthorizationFail](../../models/apiserviceidauthauthorizationfail.md) | :heavy_check_mark:                                                                            | N/A                                                                                           |