# BackchannelAuthenticationIssueApiRequestBody

An object containing schema data

## Example Usage

```typescript
import { BackchannelAuthenticationIssueApiRequestBody } from "authlete-2/models/operations";

let value: BackchannelAuthenticationIssueApiRequestBody = {
  ticket: "<value>",
};
```

## Fields

| Field                                                                 | Type                                                                  | Required                                                              | Description                                                           |
| --------------------------------------------------------------------- | --------------------------------------------------------------------- | --------------------------------------------------------------------- | --------------------------------------------------------------------- |
| `ticket`                                                              | *string*                                                              | :heavy_check_mark:                                                    | The ticket issued from Authlete's `/backchannel/authentication` API.<br/> |