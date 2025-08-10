# GetApiServiceIdAuthAuthorizationTicketInfoRequest

## Example Usage

```typescript
import { GetApiServiceIdAuthAuthorizationTicketInfoRequest } from "authlete-2/models/operations";

let value: GetApiServiceIdAuthAuthorizationTicketInfoRequest = {
  serviceId: "<id>",
  ticket: "<value>",
};
```

## Fields

| Field                                   | Type                                    | Required                                | Description                             |
| --------------------------------------- | --------------------------------------- | --------------------------------------- | --------------------------------------- |
| `serviceId`                             | *string*                                | :heavy_check_mark:                      | N/A                                     |
| `ticket`                                | *string*                                | :heavy_check_mark:                      | Ticket issued by `/auth/authorization`. |