# VciJwksApiFormAction

The next action that the implementation of the JWK Set document
endpoint of the credential issuer should take after getting a
response from Authlete's `/vci/jwks` API.


## Example Usage

```typescript
import { VciJwksApiFormAction } from "authlete-2/models/operations";

let value: VciJwksApiFormAction = "INTERNAL_SERVER_ERROR";
```

## Values

```typescript
"INTERNAL_SERVER_ERROR" | "BAD_REQUEST" | "CREATED" | "UNAUTHORIZED" | "FORBIDDEN" | "JSON" | "JWT" | "OK"
```