# ApiServiceIdClientSecretUpdateClientIdentifie

An object containing api_serviceid_client_secret_update_clientidentifie data

## Example Usage

```typescript
import { ApiServiceIdClientSecretUpdateClientIdentifie } from "authlete-2/models";

let value: ApiServiceIdClientSecretUpdateClientIdentifie = {
  clientSecret: "<value>",
};
```

## Fields

| Field                                                                                                                                                         | Type                                                                                                                                                          | Required                                                                                                                                                      | Description                                                                                                                                                   |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `clientSecret`                                                                                                                                                | *string*                                                                                                                                                      | :heavy_check_mark:                                                                                                                                            | The new value of the client secret. Valid characters for a client secret are `A-Z`, `a-z`, `0-9`,<br/>`-`, and `_`. The maximum length of a client secret is 86.<br/> |