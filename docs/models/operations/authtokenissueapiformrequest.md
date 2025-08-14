# AuthTokenIssueApiFormRequest

## Example Usage

```typescript
import { AuthTokenIssueApiFormRequest } from "authlete-typescript-sdk/models/operations";

let value: AuthTokenIssueApiFormRequest = {
  serviceId: "<id>",
  tokenIssueRequest: {},
};
```

## Fields

| Field                                                         | Type                                                          | Required                                                      | Description                                                   |
| ------------------------------------------------------------- | ------------------------------------------------------------- | ------------------------------------------------------------- | ------------------------------------------------------------- |
| `serviceId`                                                   | *string*                                                      | :heavy_check_mark:                                            | A service ID.                                                 |
| `tokenIssueRequest`                                           | [models.TokenIssueRequest](../../models/tokenissuerequest.md) | :heavy_check_mark:                                            | N/A                                                           |