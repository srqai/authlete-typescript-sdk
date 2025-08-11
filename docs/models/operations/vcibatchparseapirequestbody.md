# VciBatchParseApiRequestBody

An object containing schema data

## Example Usage

```typescript
import { VciBatchParseApiRequestBody } from "authlete-typescript-sdk/models/operations";

let value: VciBatchParseApiRequestBody = {};
```

## Fields

| Field                                                         | Type                                                          | Required                                                      | Description                                                   |
| ------------------------------------------------------------- | ------------------------------------------------------------- | ------------------------------------------------------------- | ------------------------------------------------------------- |
| `accessToken`                                                 | *string*                                                      | :heavy_minus_sign:                                            | The access token that came along with the credential request. |
| `requestContent`                                              | *string*                                                      | :heavy_minus_sign:                                            | The message body of the batch credential request.             |