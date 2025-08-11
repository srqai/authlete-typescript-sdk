# VciDeferredParseApiRequestBody

An object containing schema data

## Example Usage

```typescript
import { VciDeferredParseApiRequestBody } from "authlete-typescript-sdk/models/operations";

let value: VciDeferredParseApiRequestBody = {};
```

## Fields

| Field                                                                  | Type                                                                   | Required                                                               | Description                                                            |
| ---------------------------------------------------------------------- | ---------------------------------------------------------------------- | ---------------------------------------------------------------------- | ---------------------------------------------------------------------- |
| `accessToken`                                                          | *string*                                                               | :heavy_minus_sign:                                                     | The access token that came along with the deferred credential request. |
| `requestContent`                                                       | *string*                                                               | :heavy_minus_sign:                                                     | The message body of the deferred credential request.                   |