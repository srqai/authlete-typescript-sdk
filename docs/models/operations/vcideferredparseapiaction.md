# VciDeferredParseApiAction

The next action that the deferred credential endpoint should take.

## Example Usage

```typescript
import { VciDeferredParseApiAction } from "authlete-2/models/operations";

let value: VciDeferredParseApiAction = "JWT";
```

## Values

```typescript
"INTERNAL_SERVER_ERROR" | "BAD_REQUEST" | "CREATED" | "UNAUTHORIZED" | "FORBIDDEN" | "JSON" | "JWT" | "OK"
```