# VciOfferCreateApiFormResponse

Successful operation

## Example Usage

```typescript
import { VciOfferCreateApiFormResponse } from "authlete-typescript-sdk/models/operations";

let value: VciOfferCreateApiFormResponse = {};
```

## Fields

| Field                                                                                            | Type                                                                                             | Required                                                                                         | Description                                                                                      |
| ------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------ |
| `resultCode`                                                                                     | *string*                                                                                         | :heavy_minus_sign:                                                                               | The code which represents the result of the API call.                                            |
| `resultMessage`                                                                                  | *string*                                                                                         | :heavy_minus_sign:                                                                               | A short message which explains the result of the API call.                                       |
| `action`                                                                                         | [operations.VciOfferCreateApiFormAction](../../models/operations/vcioffercreateapiformaction.md) | :heavy_minus_sign:                                                                               | The result of the `/vci/offer/create` API call.                                                  |
| `info`                                                                                           | [models.CredentialOfferInfo](../../models/credentialofferinfo.md)                                | :heavy_minus_sign:                                                                               | N/A                                                                                              |