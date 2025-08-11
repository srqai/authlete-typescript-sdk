# AuthTokenGetListApiResponse

An object containing schema data

## Example Usage

```typescript
import { AuthTokenGetListApiResponse } from "authlete-2/models/operations";

let value: AuthTokenGetListApiResponse = {};
```

## Fields

| Field                                                                                        | Type                                                                                         | Required                                                                                     | Description                                                                                  |
| -------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------- |
| `start`                                                                                      | *number*                                                                                     | :heavy_minus_sign:                                                                           | Start index of search results (inclusive).<br/>                                              |
| `end`                                                                                        | *number*                                                                                     | :heavy_minus_sign:                                                                           | End index of search results (exclusive).<br/>                                                |
| `totalCount`                                                                                 | *number*                                                                                     | :heavy_minus_sign:                                                                           | Unique ID of a client developer.<br/>                                                        |
| `client`                                                                                     | [operations.AuthTokenGetListApiClient](../../models/operations/authtokengetlistapiclient.md) | :heavy_minus_sign:                                                                           | An object containing client data                                                             |
| `subject`                                                                                    | *string*                                                                                     | :heavy_minus_sign:                                                                           | Unique user ID of an end-user.<br/>                                                          |
| `accessTokens`                                                                               | [models.AccessToken](../../models/accesstoken.md)[]                                          | :heavy_minus_sign:                                                                           | An array of access tokens.<br/>                                                              |