# AuthAuthorizationApiAction

The next action that the authorization server implementation should take.

## Example Usage

```typescript
import { AuthAuthorizationApiAction } from "authlete-2/models/operations";

let value: AuthAuthorizationApiAction = "NO_INTERACTION";
```

## Values

```typescript
"INTERNAL_SERVER_ERROR" | "BAD_REQUEST" | "LOCATION" | "FORM" | "NO_INTERACTION" | "INTERACTION"
```