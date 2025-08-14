# AuthIntrospectionStandardApiFormRequest

## Example Usage

```typescript
import { AuthIntrospectionStandardApiFormRequest } from "authlete-typescript-sdk/models/operations";

let value: AuthIntrospectionStandardApiFormRequest = {
  serviceId: "<id>",
  introspectionStandardRequest: {},
};
```

## Fields

| Field                                                                               | Type                                                                                | Required                                                                            | Description                                                                         |
| ----------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------- |
| `serviceId`                                                                         | *string*                                                                            | :heavy_check_mark:                                                                  | A service ID.                                                                       |
| `introspectionStandardRequest`                                                      | [models.IntrospectionStandardRequest](../../models/introspectionstandardrequest.md) | :heavy_check_mark:                                                                  | N/A                                                                                 |