# ClientRegistrationDeleteApiRequest

## Example Usage

```typescript
import { ClientRegistrationDeleteApiRequest } from "authlete-2/models/operations";

let value: ClientRegistrationDeleteApiRequest = {
  serviceId: "<id>",
  requestBody: {
    clientId: 251281,
    token: "<value>",
  },
};
```

## Fields

| Field                                                                                                                  | Type                                                                                                                   | Required                                                                                                               | Description                                                                                                            |
| ---------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------- |
| `serviceId`                                                                                                            | *string*                                                                                                               | :heavy_check_mark:                                                                                                     | A service ID.                                                                                                          |
| `requestBody`                                                                                                          | [operations.ClientRegistrationDeleteApiRequestBody](../../models/operations/clientregistrationdeleteapirequestbody.md) | :heavy_check_mark:                                                                                                     | N/A                                                                                                                    |