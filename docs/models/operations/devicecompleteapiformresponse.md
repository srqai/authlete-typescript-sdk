# DeviceCompleteApiFormResponse

An object containing schema data

## Example Usage

```typescript
import { DeviceCompleteApiFormResponse } from "authlete-typescript-sdk/models/operations";

let value: DeviceCompleteApiFormResponse = {};
```

## Fields

| Field                                                                                            | Type                                                                                             | Required                                                                                         | Description                                                                                      |
| ------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------ |
| `resultCode`                                                                                     | *string*                                                                                         | :heavy_minus_sign:                                                                               | The code which represents the result of the API call.                                            |
| `resultMessage`                                                                                  | *string*                                                                                         | :heavy_minus_sign:                                                                               | A short message which explains the result of the API call.                                       |
| `action`                                                                                         | [operations.DeviceCompleteApiFormAction](../../models/operations/devicecompleteapiformaction.md) | :heavy_minus_sign:                                                                               | The next action that the authorization server implementation should take.<br/>                   |