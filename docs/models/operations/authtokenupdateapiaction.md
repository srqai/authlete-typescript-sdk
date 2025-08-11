# AuthTokenUpdateApiAction

The next action that the authorization server implementation should take.

## Example Usage

```typescript
import { AuthTokenUpdateApiAction } from "authlete-2/models/operations";

let value: AuthTokenUpdateApiAction = "BAD_REQUEST";
```

## Values

```typescript
"INTERNAL_SERVER_ERROR" | "BAD_REQUEST" | "CREATED" | "UNAUTHORIZED" | "FORBIDDEN" | "JSON" | "JWT" | "OK"
```