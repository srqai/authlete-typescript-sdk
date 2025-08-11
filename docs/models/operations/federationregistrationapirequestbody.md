# FederationRegistrationApiRequestBody

An object containing schema data

## Example Usage

```typescript
import { FederationRegistrationApiRequestBody } from "authlete-2/models/operations";

let value: FederationRegistrationApiRequestBody = {};
```

## Fields

| Field                                         | Type                                          | Required                                      | Description                                   |
| --------------------------------------------- | --------------------------------------------- | --------------------------------------------- | --------------------------------------------- |
| `entityConfiguration`                         | *string*                                      | :heavy_minus_sign:                            | The entity configuration of a relying party.<br/> |
| `trustChain`                                  | *string*                                      | :heavy_minus_sign:                            | The trust chain of a relying party.<br/>      |