# VciMetadataApiFormAction

The next action that the implementation of the credential issuer
metadata endpoint (`/.well-known/openid-credential-issuer`)
should take after getting a response from Authlete's
`/vci/metadata` API.


## Example Usage

```typescript
import { VciMetadataApiFormAction } from "authlete-typescript-sdk/models/operations";

let value: VciMetadataApiFormAction = "JWT";
```

## Values

```typescript
"INTERNAL_SERVER_ERROR" | "BAD_REQUEST" | "CREATED" | "UNAUTHORIZED" | "FORBIDDEN" | "JSON" | "JWT" | "OK"
```