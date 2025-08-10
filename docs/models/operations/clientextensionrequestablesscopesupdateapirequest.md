# ClientExtensionRequestablesScopesUpdateApiRequest

## Example Usage

```typescript
import { ClientExtensionRequestablesScopesUpdateApiRequest } from "authlete-2/models/operations";

let value: ClientExtensionRequestablesScopesUpdateApiRequest = {
  serviceId: "<id>",
  clientId: "<id>",
  requestBody: {},
};
```

## Fields

| Field                                                                                                                                                | Type                                                                                                                                                 | Required                                                                                                                                             | Description                                                                                                                                          |
| ---------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------- |
| `serviceId`                                                                                                                                          | *string*                                                                                                                                             | :heavy_check_mark:                                                                                                                                   | A service ID.                                                                                                                                        |
| `clientId`                                                                                                                                           | *string*                                                                                                                                             | :heavy_check_mark:                                                                                                                                   | A client ID.<br/>                                                                                                                                    |
| `requestBody`                                                                                                                                        | [operations.ClientExtensionRequestablesScopesUpdateApiRequestBody](../../models/operations/clientextensionrequestablesscopesupdateapirequestbody.md) | :heavy_check_mark:                                                                                                                                   | N/A                                                                                                                                                  |