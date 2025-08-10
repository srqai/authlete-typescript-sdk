# AuthUserinfoIssueApiRequest

## Example Usage

```typescript
import { AuthUserinfoIssueApiRequest } from "authlete-2/models/operations";

let value: AuthUserinfoIssueApiRequest = {
  serviceId: "<id>",
  requestBody: {
    token: "<value>",
  },
};
```

## Fields

| Field                                                                                                    | Type                                                                                                     | Required                                                                                                 | Description                                                                                              |
| -------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------- |
| `serviceId`                                                                                              | *string*                                                                                                 | :heavy_check_mark:                                                                                       | A service ID.                                                                                            |
| `requestBody`                                                                                            | [operations.AuthUserinfoIssueApiRequestBody](../../models/operations/authuserinfoissueapirequestbody.md) | :heavy_check_mark:                                                                                       | N/A                                                                                                      |