# VciMetadataApiRequest

## Example Usage

```typescript
import { VciMetadataApiRequest } from "authlete-typescript-sdk/models/operations";

let value: VciMetadataApiRequest = {
  serviceId: "<id>",
  requestBody: {
    pretty: false,
  },
};
```

## Fields

| Field                                                                                        | Type                                                                                         | Required                                                                                     | Description                                                                                  |
| -------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------- |
| `serviceId`                                                                                  | *string*                                                                                     | :heavy_check_mark:                                                                           | A service ID.                                                                                |
| `requestBody`                                                                                | [operations.VciMetadataApiRequestBody](../../models/operations/vcimetadataapirequestbody.md) | :heavy_check_mark:                                                                           | N/A                                                                                          |