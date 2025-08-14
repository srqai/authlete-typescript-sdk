# VciBatchIssueApiRequestBody

## Example Usage

```typescript
import { VciBatchIssueApiRequestBody } from "authlete-typescript-sdk/models/operations";

let value: VciBatchIssueApiRequestBody = {};
```

## Fields

| Field                                                                       | Type                                                                        | Required                                                                    | Description                                                                 |
| --------------------------------------------------------------------------- | --------------------------------------------------------------------------- | --------------------------------------------------------------------------- | --------------------------------------------------------------------------- |
| `accessToken`                                                               | *string*                                                                    | :heavy_minus_sign:                                                          | The access token that came along with the credential request.               |
| `orders`                                                                    | [models.CredentialIssuanceOrder](../../models/credentialissuanceorder.md)[] | :heavy_minus_sign:                                                          | The instructions for issuance of credentials and/or transaction IDs.        |