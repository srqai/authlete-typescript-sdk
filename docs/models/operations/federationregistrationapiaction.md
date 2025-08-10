# FederationRegistrationApiAction

The next action that the authorization server implementation should take.

## Example Usage

```typescript
import { FederationRegistrationApiAction } from "authlete-2/models/operations";

let value: FederationRegistrationApiAction = "NOT_FOUND";
```

## Values

```typescript
"OK" | "BAD_REQUEST" | "NOT_FOUND" | "INTERNAL_SERVER_ERROR"
```