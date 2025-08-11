# AuthTokenFailApiAction

The next action that the authorization server implementation should take.

## Example Usage

```typescript
import { AuthTokenFailApiAction } from "authlete-typescript-sdk/models/operations";

let value: AuthTokenFailApiAction = "UNAUTHORIZED";
```

## Values

```typescript
"INTERNAL_SERVER_ERROR" | "BAD_REQUEST" | "CREATED" | "UNAUTHORIZED" | "FORBIDDEN" | "JSON" | "JWT" | "OK"
```