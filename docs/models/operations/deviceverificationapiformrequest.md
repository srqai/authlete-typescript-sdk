# DeviceVerificationApiFormRequest

## Example Usage

```typescript
import { DeviceVerificationApiFormRequest } from "authlete-typescript-sdk/models/operations";

let value: DeviceVerificationApiFormRequest = {
  serviceId: "<id>",
  apiServiceIdDeviceVerification: {
    userCode: "<value>",
  },
};
```

## Fields

| Field                                                                                   | Type                                                                                    | Required                                                                                | Description                                                                             |
| --------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------- |
| `serviceId`                                                                             | *string*                                                                                | :heavy_check_mark:                                                                      | A service ID.                                                                           |
| `apiServiceIdDeviceVerification`                                                        | [models.ApiServiceIdDeviceVerification](../../models/apiserviceiddeviceverification.md) | :heavy_check_mark:                                                                      | N/A                                                                                     |