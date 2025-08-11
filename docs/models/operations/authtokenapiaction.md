# AuthTokenApiAction

The next action that the authorization server implementation should take.

## Example Usage

```typescript
import { AuthTokenApiAction } from "authlete-2/models/operations";

let value: AuthTokenApiAction = "UNAUTHORIZED";
```

## Values

```typescript
"INTERNAL_SERVER_ERROR" | "BAD_REQUEST" | "CREATED" | "UNAUTHORIZED" | "FORBIDDEN" | "JSON" | "JWT" | "OK"
```