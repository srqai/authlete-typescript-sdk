# AuthIntrospectionApiFormRequest

## Example Usage

```typescript
import { AuthIntrospectionApiFormRequest } from "authlete-2/models/operations";

let value: AuthIntrospectionApiFormRequest = {
  serviceId: "<id>",
  apiServiceIdAuthIntrospection: {
    token: "<value>",
  },
};
```

## Fields

| Field                                                                                 | Type                                                                                  | Required                                                                              | Description                                                                           |
| ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- |
| `serviceId`                                                                           | *string*                                                                              | :heavy_check_mark:                                                                    | A service ID.                                                                         |
| `apiServiceIdAuthIntrospection`                                                       | [models.ApiServiceIdAuthIntrospection](../../models/apiserviceidauthintrospection.md) | :heavy_check_mark:                                                                    | N/A                                                                                   |