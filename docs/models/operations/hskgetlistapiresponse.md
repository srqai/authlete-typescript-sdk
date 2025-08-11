# HskGetListApiResponse

An object containing schema data

## Example Usage

```typescript
import { HskGetListApiResponse } from "authlete-typescript-sdk/models/operations";

let value: HskGetListApiResponse = {};
```

## Fields

| Field                                                                            | Type                                                                             | Required                                                                         | Description                                                                      |
| -------------------------------------------------------------------------------- | -------------------------------------------------------------------------------- | -------------------------------------------------------------------------------- | -------------------------------------------------------------------------------- |
| `resultCode`                                                                     | *string*                                                                         | :heavy_minus_sign:                                                               | The code which represents the result of the API call.                            |
| `resultMessage`                                                                  | *string*                                                                         | :heavy_minus_sign:                                                               | A short message which explains the result of the API call.                       |
| `action`                                                                         | [operations.HskGetListApiAction](../../models/operations/hskgetlistapiaction.md) | :heavy_minus_sign:                                                               | Result of the API call                                                           |
| `hsks`                                                                           | [models.Hsk](../../models/hsk.md)[]                                              | :heavy_minus_sign:                                                               | List of HSK                                                                      |