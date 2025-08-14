# AuthIntrospectionApiFormRequest

## Example Usage

```typescript
import { AuthIntrospectionApiFormRequest } from "authlete-typescript-sdk/models/operations";

let value: AuthIntrospectionApiFormRequest = {
  serviceId: "<id>",
  introspectionRequest: {},
};
```

## Fields

| Field                                                               | Type                                                                | Required                                                            | Description                                                         |
| ------------------------------------------------------------------- | ------------------------------------------------------------------- | ------------------------------------------------------------------- | ------------------------------------------------------------------- |
| `serviceId`                                                         | *string*                                                            | :heavy_check_mark:                                                  | A service ID.                                                       |
| `introspectionRequest`                                              | [models.IntrospectionRequest](../../models/introspectionrequest.md) | :heavy_check_mark:                                                  | N/A                                                                 |