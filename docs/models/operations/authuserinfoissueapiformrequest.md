# AuthUserinfoIssueApiFormRequest

## Example Usage

```typescript
import { AuthUserinfoIssueApiFormRequest } from "authlete-typescript-sdk/models/operations";

let value: AuthUserinfoIssueApiFormRequest = {
  serviceId: "<id>",
  apiServiceIdAuthUserinfoIssue: {
    token: "<value>",
  },
};
```

## Fields

| Field                                                                                 | Type                                                                                  | Required                                                                              | Description                                                                           |
| ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- |
| `serviceId`                                                                           | *string*                                                                              | :heavy_check_mark:                                                                    | A service ID.                                                                         |
| `apiServiceIdAuthUserinfoIssue`                                                       | [models.ApiServiceIdAuthUserinfoIssue](../../models/apiserviceidauthuserinfoissue.md) | :heavy_check_mark:                                                                    | N/A                                                                                   |