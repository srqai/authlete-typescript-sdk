# VciBatchParseApiFormResponse

Successful operation

## Example Usage

```typescript
import { VciBatchParseApiFormResponse } from "authlete-typescript-sdk/models/operations";

let value: VciBatchParseApiFormResponse = {};
```

## Fields

| Field                                                                                          | Type                                                                                           | Required                                                                                       | Description                                                                                    |
| ---------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------- |
| `resultCode`                                                                                   | *string*                                                                                       | :heavy_minus_sign:                                                                             | The code which represents the result of the API call.                                          |
| `resultMessage`                                                                                | *string*                                                                                       | :heavy_minus_sign:                                                                             | A short message which explains the result of the API call.                                     |
| `action`                                                                                       | [operations.VciBatchParseApiFormAction](../../models/operations/vcibatchparseapiformaction.md) | :heavy_minus_sign:                                                                             | The next action that the batch credential endpoint should take.                                |
| `responseContent`                                                                              | *string*                                                                                       | :heavy_minus_sign:                                                                             | The content of the response to the request sender.                                             |
| `info`                                                                                         | [models.CredentialRequestInfo](../../models/credentialrequestinfo.md)[]                        | :heavy_minus_sign:                                                                             | Information about the credential requests in the batch credential<br/>request.<br/>            |