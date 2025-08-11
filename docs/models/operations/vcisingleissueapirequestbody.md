# VciSingleIssueApiRequestBody

An object containing schema data

## Example Usage

```typescript
import { VciSingleIssueApiRequestBody } from "authlete-typescript-sdk/models/operations";

let value: VciSingleIssueApiRequestBody = {};
```

## Fields

| Field                                                                     | Type                                                                      | Required                                                                  | Description                                                               |
| ------------------------------------------------------------------------- | ------------------------------------------------------------------------- | ------------------------------------------------------------------------- | ------------------------------------------------------------------------- |
| `accessToken`                                                             | *string*                                                                  | :heavy_minus_sign:                                                        | The access token that came along with the credential request.             |
| `order`                                                                   | [models.CredentialIssuanceOrder](../../models/credentialissuanceorder.md) | :heavy_minus_sign:                                                        | An object containing credentialissuanceorder data                         |