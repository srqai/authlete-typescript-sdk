# AuthIntrospectionStandardApiFormResponse

Successful operation

## Example Usage

```typescript
import { AuthIntrospectionStandardApiFormResponse } from "authlete-typescript-sdk/models/operations";

let value: AuthIntrospectionStandardApiFormResponse = {};
```

## Fields

| Field                                                                                                                  | Type                                                                                                                   | Required                                                                                                               | Description                                                                                                            |
| ---------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------- |
| `resultCode`                                                                                                           | *string*                                                                                                               | :heavy_minus_sign:                                                                                                     | The code which represents the result of the API call.                                                                  |
| `resultMessage`                                                                                                        | *string*                                                                                                               | :heavy_minus_sign:                                                                                                     | A short message which explains the result of the API call.                                                             |
| `action`                                                                                                               | [operations.AuthIntrospectionStandardApiFormAction](../../models/operations/authintrospectionstandardapiformaction.md) | :heavy_minus_sign:                                                                                                     | The next action that the authorization server implementation should take.                                              |
| `responseContent`                                                                                                      | *string*                                                                                                               | :heavy_minus_sign:                                                                                                     | The content that the authorization server implementation is to return to the client<br/>application.<br/>              |