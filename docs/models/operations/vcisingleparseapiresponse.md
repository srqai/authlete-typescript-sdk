# VciSingleParseApiResponse

Successful operation

## Example Usage

```typescript
import { VciSingleParseApiResponse } from "authlete-typescript-sdk/models/operations";

let value: VciSingleParseApiResponse = {};
```

## Fields

| Field                                                                                    | Type                                                                                     | Required                                                                                 | Description                                                                              |
| ---------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------- |
| `resultCode`                                                                             | *string*                                                                                 | :heavy_minus_sign:                                                                       | The code which represents the result of the API call.                                    |
| `resultMessage`                                                                          | *string*                                                                                 | :heavy_minus_sign:                                                                       | A short message which explains the result of the API call.                               |
| `action`                                                                                 | [operations.VciSingleParseApiAction](../../models/operations/vcisingleparseapiaction.md) | :heavy_minus_sign:                                                                       | The next action that the credential endpoint should take.                                |
| `responseContent`                                                                        | *string*                                                                                 | :heavy_minus_sign:                                                                       | The content of the response to the request sender.                                       |
| `info`                                                                                   | [models.CredentialRequestInfo](../../models/credentialrequestinfo.md)                    | :heavy_minus_sign:                                                                       | N/A                                                                                      |