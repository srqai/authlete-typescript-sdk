# GetApiServiceIdAuthAuthorizationTicketInfoResponse

Successful operation

## Example Usage

```typescript
import { GetApiServiceIdAuthAuthorizationTicketInfoResponse } from "authlete-typescript-sdk/models/operations";

let value: GetApiServiceIdAuthAuthorizationTicketInfoResponse = {};
```

## Fields

| Field                                                                                                                                      | Type                                                                                                                                       | Required                                                                                                                                   | Description                                                                                                                                |
| ------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------ |
| `info`                                                                                                                                     | *string*                                                                                                                                   | :heavy_minus_sign:                                                                                                                         | Information about the ticket.                                                                                                              |
| `action`                                                                                                                                   | [operations.GetApiServiceIdAuthAuthorizationTicketInfoAction](../../models/operations/getapiserviceidauthauthorizationticketinfoaction.md) | :heavy_minus_sign:                                                                                                                         | The result of the `/auth/authorization/ticket/info` API call.                                                                              |
| `resultCode`                                                                                                                               | *string*                                                                                                                                   | :heavy_minus_sign:                                                                                                                         | The code which represents the result of the API call.                                                                                      |
| `resultMessage`                                                                                                                            | *string*                                                                                                                                   | :heavy_minus_sign:                                                                                                                         | A short message which explains the result of the API call.                                                                                 |