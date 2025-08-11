# VciJwtissuerApiFormRequest

## Example Usage

```typescript
import { VciJwtissuerApiFormRequest } from "authlete-typescript-sdk/models/operations";

let value: VciJwtissuerApiFormRequest = {
  serviceId: "<id>",
  apiServiceIdVciJwtissuer: {
    pretty: false,
  },
};
```

## Fields

| Field                                                                       | Type                                                                        | Required                                                                    | Description                                                                 |
| --------------------------------------------------------------------------- | --------------------------------------------------------------------------- | --------------------------------------------------------------------------- | --------------------------------------------------------------------------- |
| `serviceId`                                                                 | *string*                                                                    | :heavy_check_mark:                                                          | A service ID.                                                               |
| `apiServiceIdVciJwtissuer`                                                  | [models.ApiServiceIdVciJwtissuer](../../models/apiserviceidvcijwtissuer.md) | :heavy_check_mark:                                                          | N/A                                                                         |