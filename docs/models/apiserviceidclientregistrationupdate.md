# ApiServiceIdClientRegistrationUpdate

An object containing api_serviceid_client_registration_update data

## Example Usage

```typescript
import { ApiServiceIdClientRegistrationUpdate } from "authlete-2/models";

let value: ApiServiceIdClientRegistrationUpdate = {
  clientId: 904520,
  token: "<value>",
  json: "{key: 3378765542787724, key1: null, key2: \"<value>\"}",
};
```

## Fields

| Field                                                                                                                                                          | Type                                                                                                                                                           | Required                                                                                                                                                       | Description                                                                                                                                                    |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `clientId`                                                                                                                                                     | *number*                                                                                                                                                       | :heavy_check_mark:                                                                                                                                             | Client ID.<br/>                                                                                                                                                |
| `token`                                                                                                                                                        | *string*                                                                                                                                                       | :heavy_check_mark:                                                                                                                                             | Client registration access token.<br/>                                                                                                                         |
| `json`                                                                                                                                                         | *string*                                                                                                                                                       | :heavy_check_mark:                                                                                                                                             | Client metadata in JSON format that complies with [RFC 7591](https://datatracker.ietf.org/doc/html/rfc7591)<br/>(OAuth 2.0 Dynamic Client Registration Protocol).<br/> |