# PostUpdateTicketInformationRequest

## Example Usage

```typescript
import { PostUpdateTicketInformationRequest } from "authlete-typescript-sdk/models/operations";

let value: PostUpdateTicketInformationRequest = {
  serviceId: "<id>",
  requestBody: {
    ticket: "<value>",
    info: "<value>",
  },
};
```

## Fields

| Field                                                                                                                  | Type                                                                                                                   | Required                                                                                                               | Description                                                                                                            |
| ---------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------- |
| `serviceId`                                                                                                            | *string*                                                                                                               | :heavy_check_mark:                                                                                                     | A service ID.                                                                                                          |
| `requestBody`                                                                                                          | [operations.PostUpdateTicketInformationRequestBody](../../models/operations/postupdateticketinformationrequestbody.md) | :heavy_check_mark:                                                                                                     | N/A                                                                                                                    |