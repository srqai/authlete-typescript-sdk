# ClientRegistrationDeleteApiFormRequest

## Example Usage

```typescript
import { ClientRegistrationDeleteApiFormRequest } from "authlete-2/models/operations";

let value: ClientRegistrationDeleteApiFormRequest = {
  serviceId: "<id>",
  apiServiceIdClientRegistrationDelete: {
    clientId: 755634,
    token: "<value>",
  },
};
```

## Fields

| Field                                                                                               | Type                                                                                                | Required                                                                                            | Description                                                                                         |
| --------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------- |
| `serviceId`                                                                                         | *string*                                                                                            | :heavy_check_mark:                                                                                  | A service ID.                                                                                       |
| `apiServiceIdClientRegistrationDelete`                                                              | [models.ApiServiceIdClientRegistrationDelete](../../models/apiserviceidclientregistrationdelete.md) | :heavy_check_mark:                                                                                  | N/A                                                                                                 |