# BackchannelAuthenticationApiAction

The next action that the authorization server implementation should take.

## Example Usage

```typescript
import { BackchannelAuthenticationApiAction } from "authlete-2/models/operations";

let value: BackchannelAuthenticationApiAction = "BAD_REQUEST";
```

## Values

```typescript
"INTERNAL_SERVER_ERROR" | "BAD_REQUEST" | "UNAUTHORIZED" | "USER_IDENTIFICATION"
```