# PushedAuthReqApiFormAction

The next action that the authorization server implementation should take. Any other value other than "CREATED" should be handled as unsuccessful result.

## Example Usage

```typescript
import { PushedAuthReqApiFormAction } from "authlete-typescript-sdk/models/operations";

let value: PushedAuthReqApiFormAction = "UNAUTHORIZED";
```

## Values

```typescript
"INTERNAL_SERVER_ERROR" | "BAD_REQUEST" | "CREATED" | "UNAUTHORIZED" | "FORBIDDEN" | "JSON" | "JWT" | "OK"
```