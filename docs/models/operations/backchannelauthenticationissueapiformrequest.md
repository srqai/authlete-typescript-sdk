# BackchannelAuthenticationIssueApiFormRequest

## Example Usage

```typescript
import { BackchannelAuthenticationIssueApiFormRequest } from "authlete-2/models/operations";

let value: BackchannelAuthenticationIssueApiFormRequest = {
  serviceId: "<id>",
  apiServiceIdBackchannelAuthenticationIssue: {
    ticket: "<value>",
  },
};
```

## Fields

| Field                                                                                                           | Type                                                                                                            | Required                                                                                                        | Description                                                                                                     |
| --------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------- |
| `serviceId`                                                                                                     | *string*                                                                                                        | :heavy_check_mark:                                                                                              | A service ID.                                                                                                   |
| `apiServiceIdBackchannelAuthenticationIssue`                                                                    | [models.ApiServiceIdBackchannelAuthenticationIssue](../../models/apiserviceidbackchannelauthenticationissue.md) | :heavy_check_mark:                                                                                              | N/A                                                                                                             |