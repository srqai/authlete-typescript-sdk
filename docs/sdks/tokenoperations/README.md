# TokenOperations
(*tokenOperations*)

## Overview

API endpoints for various token related operations, including creating, revoking and deleting access_tokens with specified scopes.

### Available Operations

* [authTokenGetListApi](#authtokengetlistapi) - List Issued Tokens
* [authTokenCreateApi](#authtokencreateapi) - Create Access Token
* [authTokenCreateApiForm](#authtokencreateapiform) - Create Access Token
* [authTokenUpdateApi](#authtokenupdateapi) - Update Access Token
* [authTokenUpdateApiForm](#authtokenupdateapiform) - Update Access Token
* [authTokenDeleteApi](#authtokendeleteapi) - Delete Access Token
* [authTokenRevokeApi](#authtokenrevokeapi) - Revoke Access Token
* [authTokenRevokeApiForm](#authtokenrevokeapiform) - Revoke Access Token

## authTokenGetListApi

Get the list of access tokens that are associated with the service.


### Example Usage

<!-- UsageSnippet language="typescript" operationID="auth_token_get_list_api" method="get" path="/api/{serviceId}/auth/token/get/list" -->
```typescript
import { Authlete } from "authlete-typescript-latest";

const authlete = new Authlete({
  security: {
    authlete: process.env["AUTHLETE_AUTHLETE"] ?? "",
  },
});

async function run() {
  const result = await authlete.tokenOperations.authTokenGetListApi({
    serviceId: "<id>",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { AuthleteCore } from "authlete-typescript-latest/core.js";
import { tokenOperationsAuthTokenGetListApi } from "authlete-typescript-latest/funcs/tokenOperationsAuthTokenGetListApi.js";

// Use `AuthleteCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const authlete = new AuthleteCore({
  security: {
    authlete: process.env["AUTHLETE_AUTHLETE"] ?? "",
  },
});

async function run() {
  const res = await tokenOperationsAuthTokenGetListApi(authlete, {
    serviceId: "<id>",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("tokenOperationsAuthTokenGetListApi failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.AuthTokenGetListApiRequest](../../models/operations/authtokengetlistapirequest.md)                                                                                 | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.AuthTokenGetListApiResponse](../../models/operations/authtokengetlistapiresponse.md)\>**

### Errors

| Error Type                                                        | Status Code                                                       | Content Type                                                      |
| ----------------------------------------------------------------- | ----------------------------------------------------------------- | ----------------------------------------------------------------- |
| errors.1api1infoGetResponses400Error                              | 400                                                               | application/json                                                  |
| errors.1api1infoGetResponses400ContentApplication1jsonSchemaError | 401, 403                                                          | application/json                                                  |
| errors.1api1infoGetResponses400ContentApplication1jsonSchemaError | 500                                                               | application/json                                                  |
| errors.AuthleteDefaultError                                       | 4XX, 5XX                                                          | \*/\*                                                             |

## authTokenCreateApi

Create an access token.


### Example Usage

<!-- UsageSnippet language="typescript" operationID="auth_token_create_api" method="post" path="/api/{serviceId}/auth/token/create" -->
```typescript
import { Authlete } from "authlete-typescript-latest";

const authlete = new Authlete({
  security: {
    authlete: process.env["AUTHLETE_AUTHLETE"] ?? "",
  },
});

async function run() {
  const result = await authlete.tokenOperations.authTokenCreateApi({
    serviceId: "<id>",
    requestBody: {
      grantType: "AUTHORIZATION_CODE",
      clientId: 26888344961664,
      subject: "john",
      scopes: [
        "history.read",
        "timeline.read",
      ],
    },
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { AuthleteCore } from "authlete-typescript-latest/core.js";
import { tokenOperationsAuthTokenCreateApi } from "authlete-typescript-latest/funcs/tokenOperationsAuthTokenCreateApi.js";

// Use `AuthleteCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const authlete = new AuthleteCore({
  security: {
    authlete: process.env["AUTHLETE_AUTHLETE"] ?? "",
  },
});

async function run() {
  const res = await tokenOperationsAuthTokenCreateApi(authlete, {
    serviceId: "<id>",
    requestBody: {
      grantType: "AUTHORIZATION_CODE",
      clientId: 26888344961664,
      subject: "john",
      scopes: [
        "history.read",
        "timeline.read",
      ],
    },
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("tokenOperationsAuthTokenCreateApi failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.AuthTokenCreateApiRequest](../../models/operations/authtokencreateapirequest.md)                                                                                   | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.AuthTokenCreateApiResponse](../../models/operations/authtokencreateapiresponse.md)\>**

### Errors

| Error Type                                                        | Status Code                                                       | Content Type                                                      |
| ----------------------------------------------------------------- | ----------------------------------------------------------------- | ----------------------------------------------------------------- |
| errors.1api1infoGetResponses400Error                              | 400                                                               | application/json                                                  |
| errors.1api1infoGetResponses400ContentApplication1jsonSchemaError | 401, 403                                                          | application/json                                                  |
| errors.1api1infoGetResponses400ContentApplication1jsonSchemaError | 500                                                               | application/json                                                  |
| errors.AuthleteDefaultError                                       | 4XX, 5XX                                                          | \*/\*                                                             |

## authTokenCreateApiForm

Create an access token.


### Example Usage

<!-- UsageSnippet language="typescript" operationID="auth_token_create_api_form" method="post" path="/api/{serviceId}/auth/token/create" -->
```typescript
import { Authlete } from "authlete-typescript-latest";

const authlete = new Authlete({
  security: {
    authlete: process.env["AUTHLETE_AUTHLETE"] ?? "",
  },
});

async function run() {
  const result = await authlete.tokenOperations.authTokenCreateApiForm({
    serviceId: "<id>",
    1api1ServiceId1auth1token1createPostRequestBodyContentApplication1jsonSchema: {
      grantType: "REFRESH_TOKEN",
      clientId: 987169,
    },
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { AuthleteCore } from "authlete-typescript-latest/core.js";
import { tokenOperationsAuthTokenCreateApiForm } from "authlete-typescript-latest/funcs/tokenOperationsAuthTokenCreateApiForm.js";

// Use `AuthleteCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const authlete = new AuthleteCore({
  security: {
    authlete: process.env["AUTHLETE_AUTHLETE"] ?? "",
  },
});

async function run() {
  const res = await tokenOperationsAuthTokenCreateApiForm(authlete, {
    serviceId: "<id>",
    1api1ServiceId1auth1token1createPostRequestBodyContentApplication1jsonSchema: {
      grantType: "REFRESH_TOKEN",
      clientId: 987169,
    },
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("tokenOperationsAuthTokenCreateApiForm failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.AuthTokenCreateApiFormRequest](../../models/operations/authtokencreateapiformrequest.md)                                                                           | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.AuthTokenCreateApiFormResponse](../../models/operations/authtokencreateapiformresponse.md)\>**

### Errors

| Error Type                                                        | Status Code                                                       | Content Type                                                      |
| ----------------------------------------------------------------- | ----------------------------------------------------------------- | ----------------------------------------------------------------- |
| errors.1api1infoGetResponses400Error                              | 400                                                               | application/json                                                  |
| errors.1api1infoGetResponses400ContentApplication1jsonSchemaError | 401, 403                                                          | application/json                                                  |
| errors.1api1infoGetResponses400ContentApplication1jsonSchemaError | 500                                                               | application/json                                                  |
| errors.AuthleteDefaultError                                       | 4XX, 5XX                                                          | \*/\*                                                             |

## authTokenUpdateApi

Update an access token.


### Example Usage

<!-- UsageSnippet language="typescript" operationID="auth_token_update_api" method="post" path="/api/{serviceId}/auth/token/update" -->
```typescript
import { Authlete } from "authlete-typescript-latest";

const authlete = new Authlete({
  security: {
    authlete: process.env["AUTHLETE_AUTHLETE"] ?? "",
  },
});

async function run() {
  const result = await authlete.tokenOperations.authTokenUpdateApi({
    serviceId: "<id>",
    requestBody: {
      accessToken: "Z5a40U6dWvw2gMoCOAFbZcM85q4HC0Z--0YKD9-Nf6Q",
      scopes: [
        "history.read",
      ],
    },
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { AuthleteCore } from "authlete-typescript-latest/core.js";
import { tokenOperationsAuthTokenUpdateApi } from "authlete-typescript-latest/funcs/tokenOperationsAuthTokenUpdateApi.js";

// Use `AuthleteCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const authlete = new AuthleteCore({
  security: {
    authlete: process.env["AUTHLETE_AUTHLETE"] ?? "",
  },
});

async function run() {
  const res = await tokenOperationsAuthTokenUpdateApi(authlete, {
    serviceId: "<id>",
    requestBody: {
      accessToken: "Z5a40U6dWvw2gMoCOAFbZcM85q4HC0Z--0YKD9-Nf6Q",
      scopes: [
        "history.read",
      ],
    },
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("tokenOperationsAuthTokenUpdateApi failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.AuthTokenUpdateApiRequest](../../models/operations/authtokenupdateapirequest.md)                                                                                   | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.AuthTokenUpdateApiResponse](../../models/operations/authtokenupdateapiresponse.md)\>**

### Errors

| Error Type                                                        | Status Code                                                       | Content Type                                                      |
| ----------------------------------------------------------------- | ----------------------------------------------------------------- | ----------------------------------------------------------------- |
| errors.1api1infoGetResponses400Error                              | 400                                                               | application/json                                                  |
| errors.1api1infoGetResponses400ContentApplication1jsonSchemaError | 401, 403                                                          | application/json                                                  |
| errors.1api1infoGetResponses400ContentApplication1jsonSchemaError | 500                                                               | application/json                                                  |
| errors.AuthleteDefaultError                                       | 4XX, 5XX                                                          | \*/\*                                                             |

## authTokenUpdateApiForm

Update an access token.


### Example Usage

<!-- UsageSnippet language="typescript" operationID="auth_token_update_api_form" method="post" path="/api/{serviceId}/auth/token/update" -->
```typescript
import { Authlete } from "authlete-typescript-latest";

const authlete = new Authlete({
  security: {
    authlete: process.env["AUTHLETE_AUTHLETE"] ?? "",
  },
});

async function run() {
  const result = await authlete.tokenOperations.authTokenUpdateApiForm({
    serviceId: "<id>",
    1api1ServiceId1auth1token1updatePostRequestBodyContentApplication1jsonSchema: {
      accessToken: "<value>",
    },
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { AuthleteCore } from "authlete-typescript-latest/core.js";
import { tokenOperationsAuthTokenUpdateApiForm } from "authlete-typescript-latest/funcs/tokenOperationsAuthTokenUpdateApiForm.js";

// Use `AuthleteCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const authlete = new AuthleteCore({
  security: {
    authlete: process.env["AUTHLETE_AUTHLETE"] ?? "",
  },
});

async function run() {
  const res = await tokenOperationsAuthTokenUpdateApiForm(authlete, {
    serviceId: "<id>",
    1api1ServiceId1auth1token1updatePostRequestBodyContentApplication1jsonSchema: {
      accessToken: "<value>",
    },
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("tokenOperationsAuthTokenUpdateApiForm failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.AuthTokenUpdateApiFormRequest](../../models/operations/authtokenupdateapiformrequest.md)                                                                           | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.AuthTokenUpdateApiFormResponse](../../models/operations/authtokenupdateapiformresponse.md)\>**

### Errors

| Error Type                                                        | Status Code                                                       | Content Type                                                      |
| ----------------------------------------------------------------- | ----------------------------------------------------------------- | ----------------------------------------------------------------- |
| errors.1api1infoGetResponses400Error                              | 400                                                               | application/json                                                  |
| errors.1api1infoGetResponses400ContentApplication1jsonSchemaError | 401, 403                                                          | application/json                                                  |
| errors.1api1infoGetResponses400ContentApplication1jsonSchemaError | 500                                                               | application/json                                                  |
| errors.AuthleteDefaultError                                       | 4XX, 5XX                                                          | \*/\*                                                             |

## authTokenDeleteApi

Delete an access token.


### Example Usage

<!-- UsageSnippet language="typescript" operationID="auth_token_delete_api" method="delete" path="/api/{serviceId}/auth/token/delete/{accessTokenIdentifier}" -->
```typescript
import { Authlete } from "authlete-typescript-latest";

const authlete = new Authlete({
  security: {
    authlete: process.env["AUTHLETE_AUTHLETE"] ?? "",
  },
});

async function run() {
  await authlete.tokenOperations.authTokenDeleteApi({
    serviceId: "<id>",
    accessTokenIdentifier: "<value>",
  });


}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { AuthleteCore } from "authlete-typescript-latest/core.js";
import { tokenOperationsAuthTokenDeleteApi } from "authlete-typescript-latest/funcs/tokenOperationsAuthTokenDeleteApi.js";

// Use `AuthleteCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const authlete = new AuthleteCore({
  security: {
    authlete: process.env["AUTHLETE_AUTHLETE"] ?? "",
  },
});

async function run() {
  const res = await tokenOperationsAuthTokenDeleteApi(authlete, {
    serviceId: "<id>",
    accessTokenIdentifier: "<value>",
  });
  if (res.ok) {
    const { value: result } = res;
    
  } else {
    console.log("tokenOperationsAuthTokenDeleteApi failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.AuthTokenDeleteApiRequest](../../models/operations/authtokendeleteapirequest.md)                                                                                   | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<void\>**

### Errors

| Error Type                                                        | Status Code                                                       | Content Type                                                      |
| ----------------------------------------------------------------- | ----------------------------------------------------------------- | ----------------------------------------------------------------- |
| errors.1api1infoGetResponses400Error                              | 400                                                               | application/json                                                  |
| errors.1api1infoGetResponses400ContentApplication1jsonSchemaError | 401, 403                                                          | application/json                                                  |
| errors.1api1infoGetResponses400ContentApplication1jsonSchemaError | 500                                                               | application/json                                                  |
| errors.AuthleteDefaultError                                       | 4XX, 5XX                                                          | \*/\*                                                             |

## authTokenRevokeApi

Revoke an access token.


### Example Usage

<!-- UsageSnippet language="typescript" operationID="auth_token_revoke_api" method="post" path="/api/{serviceId}/auth/token/revoke" -->
```typescript
import { Authlete } from "authlete-typescript-latest";

const authlete = new Authlete({
  security: {
    authlete: process.env["AUTHLETE_AUTHLETE"] ?? "",
  },
});

async function run() {
  const result = await authlete.tokenOperations.authTokenRevokeApi({
    serviceId: "<id>",
    requestBody: {
      accessTokenIdentifier: "Z5a40U6dWvw2gMoCOAFbZcM85q4HC0Z--0YKD9-Nf6Q",
    },
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { AuthleteCore } from "authlete-typescript-latest/core.js";
import { tokenOperationsAuthTokenRevokeApi } from "authlete-typescript-latest/funcs/tokenOperationsAuthTokenRevokeApi.js";

// Use `AuthleteCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const authlete = new AuthleteCore({
  security: {
    authlete: process.env["AUTHLETE_AUTHLETE"] ?? "",
  },
});

async function run() {
  const res = await tokenOperationsAuthTokenRevokeApi(authlete, {
    serviceId: "<id>",
    requestBody: {
      accessTokenIdentifier: "Z5a40U6dWvw2gMoCOAFbZcM85q4HC0Z--0YKD9-Nf6Q",
    },
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("tokenOperationsAuthTokenRevokeApi failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.AuthTokenRevokeApiRequest](../../models/operations/authtokenrevokeapirequest.md)                                                                                   | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.AuthTokenRevokeApiResponse](../../models/operations/authtokenrevokeapiresponse.md)\>**

### Errors

| Error Type                                                        | Status Code                                                       | Content Type                                                      |
| ----------------------------------------------------------------- | ----------------------------------------------------------------- | ----------------------------------------------------------------- |
| errors.1api1infoGetResponses400Error                              | 400                                                               | application/json                                                  |
| errors.1api1infoGetResponses400ContentApplication1jsonSchemaError | 401, 403                                                          | application/json                                                  |
| errors.1api1infoGetResponses400ContentApplication1jsonSchemaError | 500                                                               | application/json                                                  |
| errors.AuthleteDefaultError                                       | 4XX, 5XX                                                          | \*/\*                                                             |

## authTokenRevokeApiForm

Revoke an access token.


### Example Usage

<!-- UsageSnippet language="typescript" operationID="auth_token_revoke_api_form" method="post" path="/api/{serviceId}/auth/token/revoke" -->
```typescript
import { Authlete } from "authlete-typescript-latest";

const authlete = new Authlete({
  security: {
    authlete: process.env["AUTHLETE_AUTHLETE"] ?? "",
  },
});

async function run() {
  const result = await authlete.tokenOperations.authTokenRevokeApiForm({
    serviceId: "<id>",
    1api1ServiceId1auth1token1revokePostRequestBodyContentApplication1jsonSchema: {},
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { AuthleteCore } from "authlete-typescript-latest/core.js";
import { tokenOperationsAuthTokenRevokeApiForm } from "authlete-typescript-latest/funcs/tokenOperationsAuthTokenRevokeApiForm.js";

// Use `AuthleteCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const authlete = new AuthleteCore({
  security: {
    authlete: process.env["AUTHLETE_AUTHLETE"] ?? "",
  },
});

async function run() {
  const res = await tokenOperationsAuthTokenRevokeApiForm(authlete, {
    serviceId: "<id>",
    1api1ServiceId1auth1token1revokePostRequestBodyContentApplication1jsonSchema: {},
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("tokenOperationsAuthTokenRevokeApiForm failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.AuthTokenRevokeApiFormRequest](../../models/operations/authtokenrevokeapiformrequest.md)                                                                           | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.AuthTokenRevokeApiFormResponse](../../models/operations/authtokenrevokeapiformresponse.md)\>**

### Errors

| Error Type                                                        | Status Code                                                       | Content Type                                                      |
| ----------------------------------------------------------------- | ----------------------------------------------------------------- | ----------------------------------------------------------------- |
| errors.1api1infoGetResponses400Error                              | 400                                                               | application/json                                                  |
| errors.1api1infoGetResponses400ContentApplication1jsonSchemaError | 401, 403                                                          | application/json                                                  |
| errors.1api1infoGetResponses400ContentApplication1jsonSchemaError | 500                                                               | application/json                                                  |
| errors.AuthleteDefaultError                                       | 4XX, 5XX                                                          | \*/\*                                                             |