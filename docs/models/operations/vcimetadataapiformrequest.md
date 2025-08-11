# VciMetadataApiFormRequest

## Example Usage

```typescript
import { VciMetadataApiFormRequest } from "authlete-2/models/operations";

let value: VciMetadataApiFormRequest = {
  serviceId: "<id>",
  apiServiceIdVciMetadata: {
    pretty: true,
  },
};
```

## Fields

| Field                                                                     | Type                                                                      | Required                                                                  | Description                                                               |
| ------------------------------------------------------------------------- | ------------------------------------------------------------------------- | ------------------------------------------------------------------------- | ------------------------------------------------------------------------- |
| `serviceId`                                                               | *string*                                                                  | :heavy_check_mark:                                                        | A service ID.                                                             |
| `apiServiceIdVciMetadata`                                                 | [models.ApiServiceIdVciMetadata](../../models/apiserviceidvcimetadata.md) | :heavy_check_mark:                                                        | N/A                                                                       |