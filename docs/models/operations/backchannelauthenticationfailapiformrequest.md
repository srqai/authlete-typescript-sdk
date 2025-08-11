# BackchannelAuthenticationFailApiFormRequest

## Example Usage

```typescript
import { BackchannelAuthenticationFailApiFormRequest } from "authlete-typescript-sdk/models/operations";

let value: BackchannelAuthenticationFailApiFormRequest = {
  serviceId: "<id>",
  apiServiceIdBackchannelAuthenticationFail: {
    ticket: "<value>",
    reason: "UNAUTHORIZED_CLIENT",
  },
};
```

## Fields

| Field                                                                                                         | Type                                                                                                          | Required                                                                                                      | Description                                                                                                   |
| ------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------- |
| `serviceId`                                                                                                   | *string*                                                                                                      | :heavy_check_mark:                                                                                            | A service ID.                                                                                                 |
| `apiServiceIdBackchannelAuthenticationFail`                                                                   | [models.ApiServiceIdBackchannelAuthenticationFail](../../models/apiserviceidbackchannelauthenticationfail.md) | :heavy_check_mark:                                                                                            | N/A                                                                                                           |