# VciDeferredParseApiAction

The next action that the deferred credential endpoint should take.

## Example Usage

```typescript
import { VciDeferredParseApiAction } from "authlete-typescript-sdk/models/operations";

let value: VciDeferredParseApiAction = "INTERNAL_SERVER_ERROR";
```

## Values

```typescript
"OK" | "BAD_REQUEST" | "UNAUTHORIZED" | "FORBIDDEN" | "INTERNAL_SERVER_ERROR"
```