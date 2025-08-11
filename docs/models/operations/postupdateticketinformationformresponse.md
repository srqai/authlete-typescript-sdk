# PostUpdateTicketInformationFormResponse

An object containing schema data

## Example Usage

```typescript
import { PostUpdateTicketInformationFormResponse } from "authlete-2/models/operations";

let value: PostUpdateTicketInformationFormResponse = {};
```

## Fields

| Field                                                                                                                | Type                                                                                                                 | Required                                                                                                             | Description                                                                                                          |
| -------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------- |
| `info`                                                                                                               | *string*                                                                                                             | :heavy_minus_sign:                                                                                                   | Information about the ticket.                                                                                        |
| `action`                                                                                                             | [operations.PostUpdateTicketInformationFormAction](../../models/operations/postupdateticketinformationformaction.md) | :heavy_minus_sign:                                                                                                   | The result of the /auth/authorization/ticket/info API call.                                                          |
| `resultCode`                                                                                                         | *string*                                                                                                             | :heavy_minus_sign:                                                                                                   | The code which represents the result of the API call.                                                                |
| `resultMessage`                                                                                                      | *string*                                                                                                             | :heavy_minus_sign:                                                                                                   | A short message which explains the result of the API call.                                                           |