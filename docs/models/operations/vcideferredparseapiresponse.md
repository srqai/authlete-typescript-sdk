# VciDeferredParseApiResponse

An object containing schema data

## Example Usage

```typescript
import { VciDeferredParseApiResponse } from "authlete-2/models/operations";

let value: VciDeferredParseApiResponse = {};
```

## Fields

| Field                                                                                        | Type                                                                                         | Required                                                                                     | Description                                                                                  |
| -------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------- |
| `resultCode`                                                                                 | *string*                                                                                     | :heavy_minus_sign:                                                                           | The code which represents the result of the API call.                                        |
| `resultMessage`                                                                              | *string*                                                                                     | :heavy_minus_sign:                                                                           | A short message which explains the result of the API call.                                   |
| `action`                                                                                     | [operations.VciDeferredParseApiAction](../../models/operations/vcideferredparseapiaction.md) | :heavy_minus_sign:                                                                           | The next action that the deferred credential endpoint should take.                           |
| `responseContent`                                                                            | *string*                                                                                     | :heavy_minus_sign:                                                                           | The content of the response to the request sender.                                           |
| `info`                                                                                       | [models.CredentialRequestInfo](../../models/credentialrequestinfo.md)                        | :heavy_minus_sign:                                                                           | An object containing credentialrequestinfo data                                              |