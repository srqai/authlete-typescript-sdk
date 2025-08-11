# ClientRegistrationUpdateApiRequest

## Example Usage

```typescript
import { ClientRegistrationUpdateApiRequest } from "authlete-typescript-sdk/models/operations";

let value: ClientRegistrationUpdateApiRequest = {
  serviceId: "<id>",
  requestBody: {
    clientId: 189615,
    token: "<value>",
    json: "{key: 4665757877634301, key1: null, key2: \"<value>\"}",
  },
};
```

## Fields

| Field                                                                                                                  | Type                                                                                                                   | Required                                                                                                               | Description                                                                                                            |
| ---------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------- |
| `serviceId`                                                                                                            | *string*                                                                                                               | :heavy_check_mark:                                                                                                     | A service ID.                                                                                                          |
| `requestBody`                                                                                                          | [operations.ClientRegistrationUpdateApiRequestBody](../../models/operations/clientregistrationupdateapirequestbody.md) | :heavy_check_mark:                                                                                                     | N/A                                                                                                                    |