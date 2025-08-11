# ApiServiceIdGmpropertiesgmAction

The grant management action of the device authorization request.

The `grant_management_action` request parameter is defined in
[Grant Management for OAuth 2.0](https://openid.net/specs/fapi-grant-management.html).


## Example Usage

```typescript
import { ApiServiceIdGmpropertiesgmAction } from "authlete-2/models";

let value: ApiServiceIdGmpropertiesgmAction = "QUERY";
```

## Values

```typescript
"CREATE" | "QUERY" | "REPLACE" | "REVOKE" | "MERGE"
```