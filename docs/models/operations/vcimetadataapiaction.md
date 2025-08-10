# VciMetadataApiAction

The next action that the implementation of the credential issuer
metadata endpoint (`/.well-known/openid-credential-issuer`)
should take after getting a response from Authlete's
`/vci/metadata` API.


## Example Usage

```typescript
import { VciMetadataApiAction } from "authlete-2/models/operations";

let value: VciMetadataApiAction = "NOT_FOUND";
```

## Values

```typescript
"OK" | "NOT_FOUND" | "INTERNAL_SERVER_ERROR"
```