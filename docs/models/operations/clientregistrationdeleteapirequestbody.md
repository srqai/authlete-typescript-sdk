# ClientRegistrationDeleteApiRequestBody

An object containing schema data

## Example Usage

```typescript
import { ClientRegistrationDeleteApiRequestBody } from "authlete-typescript-sdk/models/operations";

let value: ClientRegistrationDeleteApiRequestBody = {
  clientId: 303257,
  token: "<value>",
};
```

## Fields

| Field                              | Type                               | Required                           | Description                        |
| ---------------------------------- | ---------------------------------- | ---------------------------------- | ---------------------------------- |
| `clientId`                         | *number*                           | :heavy_check_mark:                 | Client ID.<br/>                    |
| `token`                            | *string*                           | :heavy_check_mark:                 | Client registration access token.<br/> |