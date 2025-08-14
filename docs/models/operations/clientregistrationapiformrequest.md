# ClientRegistrationApiFormRequest

## Example Usage

```typescript
import { ClientRegistrationApiFormRequest } from "authlete-typescript-sdk/models/operations";

let value: ClientRegistrationApiFormRequest = {
  serviceId: "<id>",
  clientRegistrationRequest: {},
};
```

## Fields

| Field                                                                         | Type                                                                          | Required                                                                      | Description                                                                   |
| ----------------------------------------------------------------------------- | ----------------------------------------------------------------------------- | ----------------------------------------------------------------------------- | ----------------------------------------------------------------------------- |
| `serviceId`                                                                   | *string*                                                                      | :heavy_check_mark:                                                            | A service ID.                                                                 |
| `clientRegistrationRequest`                                                   | [models.ClientRegistrationRequest](../../models/clientregistrationrequest.md) | :heavy_check_mark:                                                            | N/A                                                                           |