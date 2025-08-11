# BackchannelAuthenticationCompleteApiFormRequest

## Example Usage

```typescript
import { BackchannelAuthenticationCompleteApiFormRequest } from "authlete-typescript-sdk/models/operations";

let value: BackchannelAuthenticationCompleteApiFormRequest = {
  serviceId: "<id>",
  apiServiceIdBackchannelAuthenticationComplete: {
    ticket: "<value>",
    result: "TRANSACTION_FAILED",
    subject: "<value>",
  },
};
```

## Fields

| Field                                                                                                                 | Type                                                                                                                  | Required                                                                                                              | Description                                                                                                           |
| --------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------- |
| `serviceId`                                                                                                           | *string*                                                                                                              | :heavy_check_mark:                                                                                                    | A service ID.                                                                                                         |
| `apiServiceIdBackchannelAuthenticationComplete`                                                                       | [models.ApiServiceIdBackchannelAuthenticationComplete](../../models/apiserviceidbackchannelauthenticationcomplete.md) | :heavy_check_mark:                                                                                                    | N/A                                                                                                                   |