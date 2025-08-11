# PostUpdateTicketInformationRequestBody

An object containing schema data

## Example Usage

```typescript
import { PostUpdateTicketInformationRequestBody } from "authlete-typescript-sdk/models/operations";

let value: PostUpdateTicketInformationRequestBody = {
  ticket: "<value>",
  info: "<value>",
};
```

## Fields

| Field                             | Type                              | Required                          | Description                       |
| --------------------------------- | --------------------------------- | --------------------------------- | --------------------------------- |
| `ticket`                          | *string*                          | :heavy_check_mark:                | The ticket.                       |
| `info`                            | *string*                          | :heavy_check_mark:                | The information about the ticket. |