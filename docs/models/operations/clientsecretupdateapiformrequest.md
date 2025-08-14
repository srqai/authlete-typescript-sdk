# ClientSecretUpdateApiFormRequest

## Example Usage

```typescript
import { ClientSecretUpdateApiFormRequest } from "authlete-typescript-sdk/models/operations";

let value: ClientSecretUpdateApiFormRequest = {
  serviceId: "<id>",
  clientIdentifier: "<value>",
  clientSecretUpdateRequest: {},
};
```

## Fields

| Field                                                                         | Type                                                                          | Required                                                                      | Description                                                                   |
| ----------------------------------------------------------------------------- | ----------------------------------------------------------------------------- | ----------------------------------------------------------------------------- | ----------------------------------------------------------------------------- |
| `serviceId`                                                                   | *string*                                                                      | :heavy_check_mark:                                                            | A service ID.                                                                 |
| `clientIdentifier`                                                            | *string*                                                                      | :heavy_check_mark:                                                            | The client ID or the client ID alias of a client.<br/>                        |
| `clientSecretUpdateRequest`                                                   | [models.ClientSecretUpdateRequest](../../models/clientsecretupdaterequest.md) | :heavy_check_mark:                                                            | N/A                                                                           |