# ApiServiceIdClientRegistration1

An object containing api_serviceid_client_registration1 data

## Example Usage

```typescript
import { ApiServiceIdClientRegistration1 } from "authlete-typescript-sdk/models";

let value: ApiServiceIdClientRegistration1 = {
  json: "{key: 7682544558645711, key1: null, key2: \"<value>\"}",
};
```

## Fields

| Field                                                                                                                                                          | Type                                                                                                                                                           | Required                                                                                                                                                       | Description                                                                                                                                                    |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `json`                                                                                                                                                         | *string*                                                                                                                                                       | :heavy_check_mark:                                                                                                                                             | Client metadata in JSON format that complies with [RFC 7591](https://datatracker.ietf.org/doc/html/rfc7591)<br/>(OAuth 2.0 Dynamic Client Registration Protocol).<br/> |
| `token`                                                                                                                                                        | *string*                                                                                                                                                       | :heavy_minus_sign:                                                                                                                                             | The client registration access token. Used only for GET, UPDATE, and DELETE requests.<br/>                                                                     |
| `clientId`                                                                                                                                                     | *number*                                                                                                                                                       | :heavy_minus_sign:                                                                                                                                             | The client's identifier. Used for GET, UPDATE, and DELETE requests<br/>                                                                                        |