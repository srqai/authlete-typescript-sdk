# AuthAuthorizationApiFormRequest

## Example Usage

```typescript
import { AuthAuthorizationApiFormRequest } from "authlete-2/models/operations";

let value: AuthAuthorizationApiFormRequest = {
  serviceId: "<id>",
  apiServiceIdAuthAuthorization: {
    parameters: "<value>",
  },
};
```

## Fields

| Field                                                                                 | Type                                                                                  | Required                                                                              | Description                                                                           |
| ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- |
| `serviceId`                                                                           | *string*                                                                              | :heavy_check_mark:                                                                    | A service ID.                                                                         |
| `apiServiceIdAuthAuthorization`                                                       | [models.ApiServiceIdAuthAuthorization](../../models/apiserviceidauthauthorization.md) | :heavy_check_mark:                                                                    | N/A                                                                                   |