# AuthIntrospectionStandardApiFormRequest

## Example Usage

```typescript
import { AuthIntrospectionStandardApiFormRequest } from "authlete-typescript-sdk/models/operations";

let value: AuthIntrospectionStandardApiFormRequest = {
  serviceId: "<id>",
  apiServiceIdAuthIntrospectionStandard: {
    parameters: "<value>",
  },
};
```

## Fields

| Field                                                                                                 | Type                                                                                                  | Required                                                                                              | Description                                                                                           |
| ----------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------- |
| `serviceId`                                                                                           | *string*                                                                                              | :heavy_check_mark:                                                                                    | A service ID.                                                                                         |
| `apiServiceIdAuthIntrospectionStandard`                                                               | [models.ApiServiceIdAuthIntrospectionStandard](../../models/apiserviceidauthintrospectionstandard.md) | :heavy_check_mark:                                                                                    | N/A                                                                                                   |