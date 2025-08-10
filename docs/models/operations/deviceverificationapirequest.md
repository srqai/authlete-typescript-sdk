# DeviceVerificationApiRequest

## Example Usage

```typescript
import { DeviceVerificationApiRequest } from "authlete-2/models/operations";

let value: DeviceVerificationApiRequest = {
  serviceId: "<id>",
  requestBody: {
    userCode: "<value>",
  },
};
```

## Fields

| Field                                                                                                      | Type                                                                                                       | Required                                                                                                   | Description                                                                                                |
| ---------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------- |
| `serviceId`                                                                                                | *string*                                                                                                   | :heavy_check_mark:                                                                                         | A service ID.                                                                                              |
| `requestBody`                                                                                              | [operations.DeviceVerificationApiRequestBody](../../models/operations/deviceverificationapirequestbody.md) | :heavy_check_mark:                                                                                         | N/A                                                                                                        |