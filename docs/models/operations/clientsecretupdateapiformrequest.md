# ClientSecretUpdateApiFormRequest

## Example Usage

```typescript
import { ClientSecretUpdateApiFormRequest } from "authlete-2/models/operations";

let value: ClientSecretUpdateApiFormRequest = {
  serviceId: "<id>",
  clientIdentifier: "<value>",
  apiServiceIdClientSecretUpdateClientIdentifie: {
    clientSecret: "<value>",
  },
};
```

## Fields

| Field                                                                                                                 | Type                                                                                                                  | Required                                                                                                              | Description                                                                                                           |
| --------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------- |
| `serviceId`                                                                                                           | *string*                                                                                                              | :heavy_check_mark:                                                                                                    | A service ID.                                                                                                         |
| `clientIdentifier`                                                                                                    | *string*                                                                                                              | :heavy_check_mark:                                                                                                    | The client ID or the client ID alias of a client.<br/>                                                                |
| `apiServiceIdClientSecretUpdateClientIdentifie`                                                                       | [models.ApiServiceIdClientSecretUpdateClientIdentifie](../../models/apiserviceidclientsecretupdateclientidentifie.md) | :heavy_check_mark:                                                                                                    | N/A                                                                                                                   |