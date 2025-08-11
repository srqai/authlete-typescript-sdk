# AuthAuthorizationIssueApiFormRequest

## Example Usage

```typescript
import { AuthAuthorizationIssueApiFormRequest } from "authlete-typescript-sdk/models/operations";

let value: AuthAuthorizationIssueApiFormRequest = {
  serviceId: "<id>",
  apiServiceIdAuthAuthorizationIssue: {
    ticket: "<value>",
    subject: "<value>",
  },
};
```

## Fields

| Field                                                                                           | Type                                                                                            | Required                                                                                        | Description                                                                                     |
| ----------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------- |
| `serviceId`                                                                                     | *string*                                                                                        | :heavy_check_mark:                                                                              | A service ID.                                                                                   |
| `apiServiceIdAuthAuthorizationIssue`                                                            | [models.ApiServiceIdAuthAuthorizationIssue](../../models/apiserviceidauthauthorizationissue.md) | :heavy_check_mark:                                                                              | N/A                                                                                             |