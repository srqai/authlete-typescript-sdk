# VciJwtissuerApiFormAction

The next action that the implementation of the JWT issuer metadata
endpoint (`/.well-known/jwt-issuer`) should take after getting
a response from Authlete's `/vci/jwtissuer` API.


## Example Usage

```typescript
import { VciJwtissuerApiFormAction } from "authlete-typescript-sdk/models/operations";

let value: VciJwtissuerApiFormAction = "FORBIDDEN";
```

## Values

```typescript
"INTERNAL_SERVER_ERROR" | "BAD_REQUEST" | "CREATED" | "UNAUTHORIZED" | "FORBIDDEN" | "JSON" | "JWT" | "OK"
```