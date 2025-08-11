# ApiServiceIdBackchannelAuthenticationIssue

An object containing api_serviceid_backchannel_authentication_issue data

## Example Usage

```typescript
import { ApiServiceIdBackchannelAuthenticationIssue } from "authlete-2/models";

let value: ApiServiceIdBackchannelAuthenticationIssue = {
  ticket: "<value>",
};
```

## Fields

| Field                                                                 | Type                                                                  | Required                                                              | Description                                                           |
| --------------------------------------------------------------------- | --------------------------------------------------------------------- | --------------------------------------------------------------------- | --------------------------------------------------------------------- |
| `ticket`                                                              | *string*                                                              | :heavy_check_mark:                                                    | The ticket issued from Authlete's `/backchannel/authentication` API.<br/> |