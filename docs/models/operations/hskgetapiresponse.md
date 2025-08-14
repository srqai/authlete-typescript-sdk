# HskGetApiResponse

Successful operation

## Example Usage

```typescript
import { HskGetApiResponse } from "authlete-typescript-sdk/models/operations";

let value: HskGetApiResponse = {};
```

## Fields

| Field                                                                       | Type                                                                        | Required                                                                    | Description                                                                 |
| --------------------------------------------------------------------------- | --------------------------------------------------------------------------- | --------------------------------------------------------------------------- | --------------------------------------------------------------------------- |
| `resultCode`                                                                | *string*                                                                    | :heavy_minus_sign:                                                          | The code which represents the result of the API call.                       |
| `resultMessage`                                                             | *string*                                                                    | :heavy_minus_sign:                                                          | A short message which explains the result of the API call.                  |
| `action`                                                                    | [operations.HskGetApiAction](../../models/operations/hskgetapiaction.md)    | :heavy_minus_sign:                                                          | Result of the API call                                                      |
| `hsk`                                                                       | [models.Hsk](../../models/hsk.md)                                           | :heavy_minus_sign:                                                          | Holds information about a key managed in an HSM (Hardware Security Module)<br/> |