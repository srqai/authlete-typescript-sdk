# ApiServiceIdAuthAuthorizationFail

An object containing api_serviceid_auth_authorization_fail data

## Example Usage

```typescript
import { ApiServiceIdAuthAuthorizationFail } from "authlete-2/models";

let value: ApiServiceIdAuthAuthorizationFail = {
  ticket: "<value>",
  reason: "INVALID_TARGET",
};
```

## Fields

| Field                                                                                                                                            | Type                                                                                                                                             | Required                                                                                                                                         | Description                                                                                                                                      |
| ------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------ |
| `ticket`                                                                                                                                         | *string*                                                                                                                                         | :heavy_check_mark:                                                                                                                               | The ticket issued from Authlete `/auth/authorization` API.<br/>                                                                                  |
| `reason`                                                                                                                                         | [models.ApiServiceIdAuthAuthorizationFailReason](../models/apiserviceidauthauthorizationfailreason.md)                                           | :heavy_check_mark:                                                                                                                               | The reason of the failure of the authorization request.<br/>For more details, see [NO_INTERACTION] in the description of `/auth/authorization` API.<br/> |
| `description`                                                                                                                                    | *string*                                                                                                                                         | :heavy_minus_sign:                                                                                                                               | The custom description about the authorization failure.<br/>                                                                                     |