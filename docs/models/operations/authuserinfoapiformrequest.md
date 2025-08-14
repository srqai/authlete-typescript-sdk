# AuthUserinfoApiFormRequest

## Example Usage

```typescript
import { AuthUserinfoApiFormRequest } from "authlete-typescript-sdk/models/operations";

let value: AuthUserinfoApiFormRequest = {
  serviceId: "<id>",
  userinfoRequest: {},
};
```

## Fields

| Field                                                     | Type                                                      | Required                                                  | Description                                               |
| --------------------------------------------------------- | --------------------------------------------------------- | --------------------------------------------------------- | --------------------------------------------------------- |
| `serviceId`                                               | *string*                                                  | :heavy_check_mark:                                        | A service ID.                                             |
| `userinfoRequest`                                         | [models.UserinfoRequest](../../models/userinforequest.md) | :heavy_check_mark:                                        | N/A                                                       |