# ClientRegistrationDeleteApiRequestBody

## Example Usage

```typescript
import { ClientRegistrationDeleteApiRequestBody } from "authlete-typescript-sdk/models/operations";

let value: ClientRegistrationDeleteApiRequestBody = {
  clientId: "<id>",
  token: "<value>",
};
```

## Fields

| Field                              | Type                               | Required                           | Description                        |
| ---------------------------------- | ---------------------------------- | ---------------------------------- | ---------------------------------- |
| `clientId`                         | *string*                           | :heavy_check_mark:                 | Client ID.<br/>                    |
| `token`                            | *string*                           | :heavy_check_mark:                 | Client registration access token.<br/> |