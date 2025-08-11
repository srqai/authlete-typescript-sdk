# ClientRegistrationGetApiRequest

## Example Usage

```typescript
import { ClientRegistrationGetApiRequest } from "authlete-typescript-sdk/models/operations";

let value: ClientRegistrationGetApiRequest = {
  serviceId: "<id>",
  apiServiceIdClientRegistration1: {
    json: "{key: 4712280260522632, key1: null, key2: \"<value>\"}",
  },
};
```

## Fields

| Field                                                                                     | Type                                                                                      | Required                                                                                  | Description                                                                               |
| ----------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------- |
| `serviceId`                                                                               | *string*                                                                                  | :heavy_check_mark:                                                                        | A service ID.                                                                             |
| `apiServiceIdClientRegistration1`                                                         | [models.ApiServiceIdClientRegistration1](../../models/apiserviceidclientregistration1.md) | :heavy_check_mark:                                                                        | N/A                                                                                       |