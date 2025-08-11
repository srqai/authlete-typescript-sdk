# DeviceCompleteApiFormRequest

## Example Usage

```typescript
import { DeviceCompleteApiFormRequest } from "authlete-2/models/operations";

let value: DeviceCompleteApiFormRequest = {
  serviceId: "<id>",
  apiServiceIdDeviceComplete: {
    userCode: "<value>",
    result: "AUTHORIZED",
    subject: "<value>",
  },
};
```

## Fields

| Field                                                                           | Type                                                                            | Required                                                                        | Description                                                                     |
| ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| `serviceId`                                                                     | *string*                                                                        | :heavy_check_mark:                                                              | A service ID.                                                                   |
| `apiServiceIdDeviceComplete`                                                    | [models.ApiServiceIdDeviceComplete](../../models/apiserviceiddevicecomplete.md) | :heavy_check_mark:                                                              | N/A                                                                             |