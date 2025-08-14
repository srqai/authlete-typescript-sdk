# PushedAuthReqApiFormRequest

## Example Usage

```typescript
import { PushedAuthReqApiFormRequest } from "authlete-typescript-sdk/models/operations";

let value: PushedAuthReqApiFormRequest = {
  serviceId: "<id>",
  pushedAuthRequest: {},
};
```

## Fields

| Field                                                         | Type                                                          | Required                                                      | Description                                                   |
| ------------------------------------------------------------- | ------------------------------------------------------------- | ------------------------------------------------------------- | ------------------------------------------------------------- |
| `serviceId`                                                   | *string*                                                      | :heavy_check_mark:                                            | A service ID.                                                 |
| `pushedAuthRequest`                                           | [models.PushedAuthRequest](../../models/pushedauthrequest.md) | :heavy_check_mark:                                            | N/A                                                           |