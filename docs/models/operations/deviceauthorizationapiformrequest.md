# DeviceAuthorizationApiFormRequest

## Example Usage

```typescript
import { DeviceAuthorizationApiFormRequest } from "authlete-typescript-sdk/models/operations";

let value: DeviceAuthorizationApiFormRequest = {
  serviceId: "<id>",
  apiServiceIdDeviceAuthorization: {
    parameters: "<value>",
  },
};
```

## Fields

| Field                                                                                     | Type                                                                                      | Required                                                                                  | Description                                                                               |
| ----------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------- |
| `serviceId`                                                                               | *string*                                                                                  | :heavy_check_mark:                                                                        | A service ID.                                                                             |
| `apiServiceIdDeviceAuthorization`                                                         | [models.ApiServiceIdDeviceAuthorization](../../models/apiserviceiddeviceauthorization.md) | :heavy_check_mark:                                                                        | N/A                                                                                       |