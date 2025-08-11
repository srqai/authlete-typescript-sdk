# ClientRegistrationUpdateApiFormRequest

## Example Usage

```typescript
import { ClientRegistrationUpdateApiFormRequest } from "authlete-2/models/operations";

let value: ClientRegistrationUpdateApiFormRequest = {
  serviceId: "<id>",
  apiServiceIdClientRegistrationUpdate: {
    clientId: 629769,
    token: "<value>",
    json: "{key: 338521626482512, key1: null, key2: \"<value>\"}",
  },
};
```

## Fields

| Field                                                                                               | Type                                                                                                | Required                                                                                            | Description                                                                                         |
| --------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------- |
| `serviceId`                                                                                         | *string*                                                                                            | :heavy_check_mark:                                                                                  | A service ID.                                                                                       |
| `apiServiceIdClientRegistrationUpdate`                                                              | [models.ApiServiceIdClientRegistrationUpdate](../../models/apiserviceidclientregistrationupdate.md) | :heavy_check_mark:                                                                                  | N/A                                                                                                 |