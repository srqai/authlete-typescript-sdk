# ClientRegistrationApiFormRequest

## Example Usage

```typescript
import { ClientRegistrationApiFormRequest } from "authlete-typescript-sdk/models/operations";

let value: ClientRegistrationApiFormRequest = {
  serviceId: "<id>",
  apiServiceIdClientRegistration: {
    json: "{key: 5409241029417244, key1: null, key2: \"<value>\"}",
  },
};
```

## Fields

| Field                                                                                   | Type                                                                                    | Required                                                                                | Description                                                                             |
| --------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------- |
| `serviceId`                                                                             | *string*                                                                                | :heavy_check_mark:                                                                      | A service ID.                                                                           |
| `apiServiceIdClientRegistration`                                                        | [models.ApiServiceIdClientRegistration](../../models/apiserviceidclientregistration.md) | :heavy_check_mark:                                                                      | N/A                                                                                     |