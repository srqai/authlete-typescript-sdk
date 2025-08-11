# PostUpdateTicketInformationFormRequest

## Example Usage

```typescript
import { PostUpdateTicketInformationFormRequest } from "authlete-2/models/operations";

let value: PostUpdateTicketInformationFormRequest = {
  serviceId: "<id>",
  apiServiceIdAuthAuthorizationTicketUpdate: {
    ticket: "<value>",
    info: "<value>",
  },
};
```

## Fields

| Field                                                                                                         | Type                                                                                                          | Required                                                                                                      | Description                                                                                                   |
| ------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------- |
| `serviceId`                                                                                                   | *string*                                                                                                      | :heavy_check_mark:                                                                                            | A service ID.                                                                                                 |
| `apiServiceIdAuthAuthorizationTicketUpdate`                                                                   | [models.ApiServiceIdAuthAuthorizationTicketUpdate](../../models/apiserviceidauthauthorizationticketupdate.md) | :heavy_check_mark:                                                                                            | N/A                                                                                                           |