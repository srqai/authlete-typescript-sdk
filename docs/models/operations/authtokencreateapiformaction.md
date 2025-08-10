# AuthTokenCreateApiFormAction

The next action that the authorization server implementation should take.

## Example Usage

```typescript
import { AuthTokenCreateApiFormAction } from "authlete-2/models/operations";

let value: AuthTokenCreateApiFormAction = "BAD_REQUEST";
```

## Values

```typescript
"INTERNAL_SERVER_ERROR" | "BAD_REQUEST" | "FORBIDDEN" | "OK"
```