# AuthTokenApiRequest

## Example Usage

```typescript
import { AuthTokenApiRequest } from "authlete-2/models/operations";

let value: AuthTokenApiRequest = {
  serviceId: "<id>",
  requestBody: {
    parameters: "<value>",
  },
};
```

## Fields

| Field                                                                                    | Type                                                                                     | Required                                                                                 | Description                                                                              |
| ---------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------- |
| `serviceId`                                                                              | *string*                                                                                 | :heavy_check_mark:                                                                       | A service ID.                                                                            |
| `requestBody`                                                                            | [operations.AuthTokenApiRequestBody](../../models/operations/authtokenapirequestbody.md) | :heavy_check_mark:                                                                       | N/A                                                                                      |