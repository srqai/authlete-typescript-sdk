# DeviceAuthorizationApiFormRequest

## Example Usage

```typescript
import { DeviceAuthorizationApiFormRequest } from "authlete-typescript-sdk/models/operations";

let value: DeviceAuthorizationApiFormRequest = {
  serviceId: "<id>",
  deviceAuthorizationRequest: {},
};
```

## Fields

| Field                                                                           | Type                                                                            | Required                                                                        | Description                                                                     |
| ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| `serviceId`                                                                     | *string*                                                                        | :heavy_check_mark:                                                              | A service ID.                                                                   |
| `deviceAuthorizationRequest`                                                    | [models.DeviceAuthorizationRequest](../../models/deviceauthorizationrequest.md) | :heavy_check_mark:                                                              | N/A                                                                             |