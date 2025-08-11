# FederationRegistrationApiFormRequest

## Example Usage

```typescript
import { FederationRegistrationApiFormRequest } from "authlete-2/models/operations";

let value: FederationRegistrationApiFormRequest = {
  serviceId: "<id>",
  apiServiceIdFederationRegistration: {},
};
```

## Fields

| Field                                                                                           | Type                                                                                            | Required                                                                                        | Description                                                                                     |
| ----------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------- |
| `serviceId`                                                                                     | *string*                                                                                        | :heavy_check_mark:                                                                              | A service ID.                                                                                   |
| `apiServiceIdFederationRegistration`                                                            | [models.ApiServiceIdFederationRegistration](../../models/apiserviceidfederationregistration.md) | :heavy_check_mark:                                                                              | N/A                                                                                             |