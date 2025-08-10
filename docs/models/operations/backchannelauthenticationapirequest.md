# BackchannelAuthenticationApiRequest

## Example Usage

```typescript
import { BackchannelAuthenticationApiRequest } from "authlete-typescript-sdk/models/operations";

let value: BackchannelAuthenticationApiRequest = {
  serviceId: "<id>",
  requestBody: {
    parameters: "<value>",
  },
};
```

## Fields

| Field                                                                                                                    | Type                                                                                                                     | Required                                                                                                                 | Description                                                                                                              |
| ------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------ |
| `serviceId`                                                                                                              | *string*                                                                                                                 | :heavy_check_mark:                                                                                                       | A service ID.                                                                                                            |
| `requestBody`                                                                                                            | [operations.BackchannelAuthenticationApiRequestBody](../../models/operations/backchannelauthenticationapirequestbody.md) | :heavy_check_mark:                                                                                                       | N/A                                                                                                                      |