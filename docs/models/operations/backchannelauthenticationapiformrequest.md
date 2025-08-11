# BackchannelAuthenticationApiFormRequest

## Example Usage

```typescript
import { BackchannelAuthenticationApiFormRequest } from "authlete-typescript-sdk/models/operations";

let value: BackchannelAuthenticationApiFormRequest = {
  serviceId: "<id>",
  apiServiceIdBackchannelAuthentication: {
    parameters: "<value>",
  },
};
```

## Fields

| Field                                                                                                 | Type                                                                                                  | Required                                                                                              | Description                                                                                           |
| ----------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------- |
| `serviceId`                                                                                           | *string*                                                                                              | :heavy_check_mark:                                                                                    | A service ID.                                                                                         |
| `apiServiceIdBackchannelAuthentication`                                                               | [models.ApiServiceIdBackchannelAuthentication](../../models/apiserviceidbackchannelauthentication.md) | :heavy_check_mark:                                                                                    | N/A                                                                                                   |