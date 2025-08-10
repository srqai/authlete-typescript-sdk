# FederationRegistrationApiFormAction

The next action that the authorization server implementation should take.

## Example Usage

```typescript
import { FederationRegistrationApiFormAction } from "authlete-2/models/operations";

let value: FederationRegistrationApiFormAction = "BAD_REQUEST";
```

## Values

```typescript
"OK" | "BAD_REQUEST" | "NOT_FOUND" | "INTERNAL_SERVER_ERROR"
```