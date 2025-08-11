# AuthTokenIssueApiFormRequest

## Example Usage

```typescript
import { AuthTokenIssueApiFormRequest } from "authlete-typescript-sdk/models/operations";

let value: AuthTokenIssueApiFormRequest = {
  serviceId: "<id>",
  apiServiceIdAuthTokenIssue: {
    ticket: "<value>",
    subject: "<value>",
  },
};
```

## Fields

| Field                                                                           | Type                                                                            | Required                                                                        | Description                                                                     |
| ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| `serviceId`                                                                     | *string*                                                                        | :heavy_check_mark:                                                              | A service ID.                                                                   |
| `apiServiceIdAuthTokenIssue`                                                    | [models.ApiServiceIdAuthTokenIssue](../../models/apiserviceidauthtokenissue.md) | :heavy_check_mark:                                                              | N/A                                                                             |