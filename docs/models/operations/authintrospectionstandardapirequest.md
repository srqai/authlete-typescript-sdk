# AuthIntrospectionStandardApiRequest

## Example Usage

```typescript
import { AuthIntrospectionStandardApiRequest } from "authlete-2/models/operations";

let value: AuthIntrospectionStandardApiRequest = {
  serviceId: "<id>",
  requestBody: {
    parameters: "<value>",
  },
};
```

## Fields

| Field                                                                                                                    | Type                                                                                                                     | Required                                                                                                                 | Description                                                                                                              |
| ------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------ |
| `serviceId`                                                                                                              | *string*                                                                                                                 | :heavy_check_mark:                                                                                                       | A service ID.                                                                                                            |
| `requestBody`                                                                                                            | [operations.AuthIntrospectionStandardApiRequestBody](../../models/operations/authintrospectionstandardapirequestbody.md) | :heavy_check_mark:                                                                                                       | N/A                                                                                                                      |