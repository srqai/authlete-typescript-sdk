# BackchannelAuthenticationFailApiRequest

## Example Usage

```typescript
import { BackchannelAuthenticationFailApiRequest } from "authlete-typescript-sdk/models/operations";

let value: BackchannelAuthenticationFailApiRequest = {
  serviceId: "<id>",
  requestBody: {
    ticket: "<value>",
    reason: "EXPIRED_LOGIN_HINT_TOKEN",
  },
};
```

## Fields

| Field                                                                                                                            | Type                                                                                                                             | Required                                                                                                                         | Description                                                                                                                      |
| -------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------- |
| `serviceId`                                                                                                                      | *string*                                                                                                                         | :heavy_check_mark:                                                                                                               | A service ID.                                                                                                                    |
| `requestBody`                                                                                                                    | [operations.BackchannelAuthenticationFailApiRequestBody](../../models/operations/backchannelauthenticationfailapirequestbody.md) | :heavy_check_mark:                                                                                                               | N/A                                                                                                                              |