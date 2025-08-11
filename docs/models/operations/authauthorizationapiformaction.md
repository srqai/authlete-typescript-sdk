# AuthAuthorizationApiFormAction

The next action that the authorization server implementation should take.

## Example Usage

```typescript
import { AuthAuthorizationApiFormAction } from "authlete-2/models/operations";

let value: AuthAuthorizationApiFormAction = "FORBIDDEN";
```

## Values

```typescript
"INTERNAL_SERVER_ERROR" | "BAD_REQUEST" | "CREATED" | "UNAUTHORIZED" | "FORBIDDEN" | "JSON" | "JWT" | "OK"
```