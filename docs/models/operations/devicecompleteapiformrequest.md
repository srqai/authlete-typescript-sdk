# DeviceCompleteApiFormRequest

## Example Usage

```typescript
import { DeviceCompleteApiFormRequest } from "authlete-typescript-sdk/models/operations";

let value: DeviceCompleteApiFormRequest = {
  serviceId: "<id>",
  deviceCompleteRequest: {},
};
```

## Fields

| Field                                                                 | Type                                                                  | Required                                                              | Description                                                           |
| --------------------------------------------------------------------- | --------------------------------------------------------------------- | --------------------------------------------------------------------- | --------------------------------------------------------------------- |
| `serviceId`                                                           | *string*                                                              | :heavy_check_mark:                                                    | A service ID.                                                         |
| `deviceCompleteRequest`                                               | [models.DeviceCompleteRequest](../../models/devicecompleterequest.md) | :heavy_check_mark:                                                    | N/A                                                                   |