# AuthUserinfoApiRequest

## Example Usage

```typescript
import { AuthUserinfoApiRequest } from "authlete-typescript-sdk/models/operations";

let value: AuthUserinfoApiRequest = {
  serviceId: "<id>",
  requestBody: {
    token: "<value>",
  },
};
```

## Fields

| Field                                                                                          | Type                                                                                           | Required                                                                                       | Description                                                                                    |
| ---------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------- |
| `serviceId`                                                                                    | *string*                                                                                       | :heavy_check_mark:                                                                             | A service ID.                                                                                  |
| `requestBody`                                                                                  | [operations.AuthUserinfoApiRequestBody](../../models/operations/authuserinfoapirequestbody.md) | :heavy_check_mark:                                                                             | N/A                                                                                            |