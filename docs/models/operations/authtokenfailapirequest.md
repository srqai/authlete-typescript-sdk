# AuthTokenFailApiRequest

## Example Usage

```typescript
import { AuthTokenFailApiRequest } from "authlete-typescript-sdk/models/operations";

let value: AuthTokenFailApiRequest = {
  serviceId: "<id>",
  requestBody: {
    ticket: "<value>",
    reason: "INVALID_RESOURCE_OWNER_CREDENTIALS",
  },
};
```

## Fields

| Field                                                                                            | Type                                                                                             | Required                                                                                         | Description                                                                                      |
| ------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------ |
| `serviceId`                                                                                      | *string*                                                                                         | :heavy_check_mark:                                                                               | A service ID.                                                                                    |
| `requestBody`                                                                                    | [operations.AuthTokenFailApiRequestBody](../../models/operations/authtokenfailapirequestbody.md) | :heavy_check_mark:                                                                               | N/A                                                                                              |