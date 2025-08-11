# ApiServiceIdVciDeferredParse

An object containing api_serviceid_vci_deferred_parse data

## Example Usage

```typescript
import { ApiServiceIdVciDeferredParse } from "authlete-2/models";

let value: ApiServiceIdVciDeferredParse = {};
```

## Fields

| Field                                                                  | Type                                                                   | Required                                                               | Description                                                            |
| ---------------------------------------------------------------------- | ---------------------------------------------------------------------- | ---------------------------------------------------------------------- | ---------------------------------------------------------------------- |
| `accessToken`                                                          | *string*                                                               | :heavy_minus_sign:                                                     | The access token that came along with the deferred credential request. |
| `requestContent`                                                       | *string*                                                               | :heavy_minus_sign:                                                     | The message body of the deferred credential request.                   |