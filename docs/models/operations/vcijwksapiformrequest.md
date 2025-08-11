# VciJwksApiFormRequest

## Example Usage

```typescript
import { VciJwksApiFormRequest } from "authlete-2/models/operations";

let value: VciJwksApiFormRequest = {
  serviceId: "<id>",
  apiServiceIdVciJwks: {
    pretty: true,
  },
};
```

## Fields

| Field                                                             | Type                                                              | Required                                                          | Description                                                       |
| ----------------------------------------------------------------- | ----------------------------------------------------------------- | ----------------------------------------------------------------- | ----------------------------------------------------------------- |
| `serviceId`                                                       | *string*                                                          | :heavy_check_mark:                                                | A service ID.                                                     |
| `apiServiceIdVciJwks`                                             | [models.ApiServiceIdVciJwks](../../models/apiserviceidvcijwks.md) | :heavy_check_mark:                                                | N/A                                                               |