# PushedAuthReqApiFormRequest

## Example Usage

```typescript
import { PushedAuthReqApiFormRequest } from "authlete-2/models/operations";

let value: PushedAuthReqApiFormRequest = {
  serviceId: "<id>",
  apiServiceIdPushedAuthReq: {
    parameters: "<value>",
  },
};
```

## Fields

| Field                                                                         | Type                                                                          | Required                                                                      | Description                                                                   |
| ----------------------------------------------------------------------------- | ----------------------------------------------------------------------------- | ----------------------------------------------------------------------------- | ----------------------------------------------------------------------------- |
| `serviceId`                                                                   | *string*                                                                      | :heavy_check_mark:                                                            | A service ID.                                                                 |
| `apiServiceIdPushedAuthReq`                                                   | [models.ApiServiceIdPushedAuthReq](../../models/apiserviceidpushedauthreq.md) | :heavy_check_mark:                                                            | N/A                                                                           |