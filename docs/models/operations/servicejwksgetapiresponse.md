# ServiceJwksGetApiResponse

An object containing schema data

## Example Usage

```typescript
import { ServiceJwksGetApiResponse } from "authlete-2/models/operations";

let value: ServiceJwksGetApiResponse = {};
```

## Fields

| Field                                                              | Type                                                               | Required                                                           | Description                                                        |
| ------------------------------------------------------------------ | ------------------------------------------------------------------ | ------------------------------------------------------------------ | ------------------------------------------------------------------ |
| `keys`                                                             | [operations.Key](../../models/operations/key.md)[]                 | :heavy_minus_sign:                                                 | An array of [JWK](https://datatracker.ietf.org/doc/html/rfc7517)s. |