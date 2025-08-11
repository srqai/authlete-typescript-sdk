# ApiServiceIdAuthTokenFail

An object containing api_serviceid_auth_token_fail data

## Example Usage

```typescript
import { ApiServiceIdAuthTokenFail } from "authlete-typescript-sdk/models";

let value: ApiServiceIdAuthTokenFail = {
  ticket: "<value>",
  reason: "INVALID_RESOURCE_OWNER_CREDENTIALS",
};
```

## Fields

| Field                                                                                  | Type                                                                                   | Required                                                                               | Description                                                                            |
| -------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------- |
| `ticket`                                                                               | *string*                                                                               | :heavy_check_mark:                                                                     | The ticket issued from Authlete `/auth/token` API.<br/>                                |
| `reason`                                                                               | [models.ApiServiceIdAuthTokenFailReason](../models/apiserviceidauthtokenfailreason.md) | :heavy_check_mark:                                                                     | The reason of the failure of the token request.<br/>                                   |