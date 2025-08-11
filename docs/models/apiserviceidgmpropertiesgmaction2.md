# ApiServiceIdGmpropertiesgmAction2

The grant management action of the device authorization request.

The `grant_management_action` request parameter is defined in
[Grant Management for OAuth 2.0](https://openid.net/specs/fapi-grant-management.html).


## Example Usage

```typescript
import { ApiServiceIdGmpropertiesgmAction2 } from "authlete-typescript-sdk/models";

let value: ApiServiceIdGmpropertiesgmAction2 = "REVOKE";
```

## Values

```typescript
"CREATE" | "QUERY" | "REPLACE" | "REVOKE" | "MERGE"
```