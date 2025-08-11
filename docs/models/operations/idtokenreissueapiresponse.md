# IdtokenReissueApiResponse

An object containing schema data

## Example Usage

```typescript
import { IdtokenReissueApiResponse } from "authlete-typescript-sdk/models/operations";

let value: IdtokenReissueApiResponse = {};
```

## Fields

| Field                                                                                                                             | Type                                                                                                                              | Required                                                                                                                          | Description                                                                                                                       |
| --------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------- |
| `resultCode`                                                                                                                      | *string*                                                                                                                          | :heavy_minus_sign:                                                                                                                | The code which represents the result of the API call.                                                                             |
| `resultMessage`                                                                                                                   | *string*                                                                                                                          | :heavy_minus_sign:                                                                                                                | A short message which explains the result of the API call.                                                                        |
| `action`                                                                                                                          | [operations.IdtokenReissueApiAction](../../models/operations/idtokenreissueapiaction.md)                                          | :heavy_minus_sign:                                                                                                                | The next action that the implementation of the token endpoint should take.                                                        |
| `responseContent`                                                                                                                 | *string*                                                                                                                          | :heavy_minus_sign:                                                                                                                | The response content that can be used as the message body of the token response that should<br/>be returned from the token endpoint.<br/> |
| `idToken`                                                                                                                         | *string*                                                                                                                          | :heavy_minus_sign:                                                                                                                | The reissued ID token<br/>                                                                                                        |