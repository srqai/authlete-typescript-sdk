# ClientAuthorizationGetListApiResponse

An object containing schema data

## Example Usage

```typescript
import { ClientAuthorizationGetListApiResponse } from "authlete-typescript-sdk/models/operations";

let value: ClientAuthorizationGetListApiResponse = {};
```

## Fields

| Field                                                                                                                 | Type                                                                                                                  | Required                                                                                                              | Description                                                                                                           |
| --------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------- |
| `start`                                                                                                               | *number*                                                                                                              | :heavy_minus_sign:                                                                                                    | Start index of search results (inclusive).<br/>                                                                       |
| `end`                                                                                                                 | *number*                                                                                                              | :heavy_minus_sign:                                                                                                    | End index of search results (exclusive).<br/>                                                                         |
| `developer`                                                                                                           | *string*                                                                                                              | :heavy_minus_sign:                                                                                                    | Unique ID of a client developer.<br/>                                                                                 |
| `subject`                                                                                                             | *string*                                                                                                              | :heavy_minus_sign:                                                                                                    | Unique user ID of an end-user.<br/>                                                                                   |
| `totalCount`                                                                                                          | *number*                                                                                                              | :heavy_minus_sign:                                                                                                    | Unique ID of a client developer.<br/>                                                                                 |
| `clients`                                                                                                             | [models.ApiServiceIdAuthTokenGetListpropertiesclient](../../models/apiserviceidauthtokengetlistpropertiesclient.md)[] | :heavy_minus_sign:                                                                                                    | An array of clients.<br/>                                                                                             |