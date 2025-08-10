# SupportedAttachment

Supported attachment types. This property corresponds to the `attachments_supported`
 server metadata which was added by the third implementer's draft of OpenID Connect
 for Identity Assurance 1.0.


## Example Usage

```typescript
import { SupportedAttachment } from "authlete-2/models";

let value: SupportedAttachment = "EMBEDDED";
```

## Values

```typescript
"EMBEDDED" | "EXTERNAL"
```