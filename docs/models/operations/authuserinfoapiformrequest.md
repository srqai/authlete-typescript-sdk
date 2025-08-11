# AuthUserinfoApiFormRequest

## Example Usage

```typescript
import { AuthUserinfoApiFormRequest } from "authlete-2/models/operations";

let value: AuthUserinfoApiFormRequest = {
  serviceId: "<id>",
  apiServiceIdAuthUserinfo: {
    token: "<value>",
  },
};
```

## Fields

| Field                                                                       | Type                                                                        | Required                                                                    | Description                                                                 |
| --------------------------------------------------------------------------- | --------------------------------------------------------------------------- | --------------------------------------------------------------------------- | --------------------------------------------------------------------------- |
| `serviceId`                                                                 | *string*                                                                    | :heavy_check_mark:                                                          | A service ID.                                                               |
| `apiServiceIdAuthUserinfo`                                                  | [models.ApiServiceIdAuthUserinfo](../../models/apiserviceidauthuserinfo.md) | :heavy_check_mark:                                                          | N/A                                                                         |