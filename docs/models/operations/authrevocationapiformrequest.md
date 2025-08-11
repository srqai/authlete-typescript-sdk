# AuthRevocationApiFormRequest

## Example Usage

```typescript
import { AuthRevocationApiFormRequest } from "authlete-2/models/operations";

let value: AuthRevocationApiFormRequest = {
  serviceId: "<id>",
  apiServiceIdAuthRevocation: {
    parameters: "<value>",
  },
};
```

## Fields

| Field                                                                           | Type                                                                            | Required                                                                        | Description                                                                     |
| ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| `serviceId`                                                                     | *string*                                                                        | :heavy_check_mark:                                                              | A service ID.                                                                   |
| `apiServiceIdAuthRevocation`                                                    | [models.ApiServiceIdAuthRevocation](../../models/apiserviceidauthrevocation.md) | :heavy_check_mark:                                                              | N/A                                                                             |