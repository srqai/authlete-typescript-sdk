# FederationRegistrationApiFormRequest

## Example Usage

```typescript
import { FederationRegistrationApiFormRequest } from "authlete-typescript-sdk/models/operations";

let value: FederationRegistrationApiFormRequest = {
  serviceId: "<id>",
  federationRegistrationRequest: {},
};
```

## Fields

| Field                                                                                 | Type                                                                                  | Required                                                                              | Description                                                                           |
| ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- |
| `serviceId`                                                                           | *string*                                                                              | :heavy_check_mark:                                                                    | A service ID.                                                                         |
| `federationRegistrationRequest`                                                       | [models.FederationRegistrationRequest](../../models/federationregistrationrequest.md) | :heavy_check_mark:                                                                    | N/A                                                                                   |