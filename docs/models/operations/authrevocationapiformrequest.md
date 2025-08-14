# AuthRevocationApiFormRequest

## Example Usage

```typescript
import { AuthRevocationApiFormRequest } from "authlete-typescript-sdk/models/operations";

let value: AuthRevocationApiFormRequest = {
  serviceId: "<id>",
  revocationRequest: {},
};
```

## Fields

| Field                                                         | Type                                                          | Required                                                      | Description                                                   |
| ------------------------------------------------------------- | ------------------------------------------------------------- | ------------------------------------------------------------- | ------------------------------------------------------------- |
| `serviceId`                                                   | *string*                                                      | :heavy_check_mark:                                            | A service ID.                                                 |
| `revocationRequest`                                           | [models.RevocationRequest](../../models/revocationrequest.md) | :heavy_check_mark:                                            | N/A                                                           |