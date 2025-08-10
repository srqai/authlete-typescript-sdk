# AuthTokenRevokeApiRequest

## Example Usage

```typescript
import { AuthTokenRevokeApiRequest } from "authlete-typescript-sdk/models/operations";

let value: AuthTokenRevokeApiRequest = {
  serviceId: "<id>",
  requestBody: {},
};
```

## Fields

| Field                                                                                                | Type                                                                                                 | Required                                                                                             | Description                                                                                          |
| ---------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------- |
| `serviceId`                                                                                          | *string*                                                                                             | :heavy_check_mark:                                                                                   | A service ID.                                                                                        |
| `requestBody`                                                                                        | [operations.AuthTokenRevokeApiRequestBody](../../models/operations/authtokenrevokeapirequestbody.md) | :heavy_check_mark:                                                                                   | N/A                                                                                                  |