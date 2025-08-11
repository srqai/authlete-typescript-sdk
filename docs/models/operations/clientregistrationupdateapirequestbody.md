# ClientRegistrationUpdateApiRequestBody

An object containing schema data

## Example Usage

```typescript
import { ClientRegistrationUpdateApiRequestBody } from "authlete-typescript-sdk/models/operations";

let value: ClientRegistrationUpdateApiRequestBody = {
  clientId: 789635,
  token: "<value>",
  json: "{key: 5008491952068490, key1: null, key2: \"<value>\"}",
};
```

## Fields

| Field                                                                                                                                                          | Type                                                                                                                                                           | Required                                                                                                                                                       | Description                                                                                                                                                    |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `clientId`                                                                                                                                                     | *number*                                                                                                                                                       | :heavy_check_mark:                                                                                                                                             | Client ID.<br/>                                                                                                                                                |
| `token`                                                                                                                                                        | *string*                                                                                                                                                       | :heavy_check_mark:                                                                                                                                             | Client registration access token.<br/>                                                                                                                         |
| `json`                                                                                                                                                         | *string*                                                                                                                                                       | :heavy_check_mark:                                                                                                                                             | Client metadata in JSON format that complies with [RFC 7591](https://datatracker.ietf.org/doc/html/rfc7591)<br/>(OAuth 2.0 Dynamic Client Registration Protocol).<br/> |