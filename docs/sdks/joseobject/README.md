# JoseObject
(*joseObject*)

## Overview

API endpoints for JOSE objects.

### Available Operations

* [joseVerifyApi](#joseverifyapi) - Verify JOSE
* [joseVerifyApiForm](#joseverifyapiform) - Verify JOSE

## joseVerifyApi

This API verifies a JOSE object.


### Example Usage

<!-- UsageSnippet language="typescript" operationID="jose_verify_api" method="post" path="/api/{serviceId}/jose/verify" -->
```typescript
import { Authlete } from "authlete-typescript-latest";

const authlete = new Authlete({
  security: {
    authlete: process.env["AUTHLETE_AUTHLETE"] ?? "",
  },
});

async function run() {
  const result = await authlete.joseObject.joseVerifyApi({
    serviceId: "<id>",
    requestBody: {
      jose: "eyJhbGciOiJFUzI1NiJ9.eyJleHAiOjE1NTk4MTE3NTAsImlzcyI6IjU3Mjk3NDA4ODY3In0K.csmdholMVcmjqHe59YWgLGNvm7I5Whp4phQCoGxyrlRGMnTgsfxtwyxBgMXQqEPD5q5k9FaEWNk37K8uAtSwrA",
      clockSkew: 100,
      clientIdentifier: "57297408867",
      signedByClient: true,
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
import { joseObjectJoseVerifyApi } from "authlete-typescript-latest/funcs/joseObjectJoseVerifyApi.js";

// Use `AuthleteCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const authlete = new AuthleteCore({
  security: {
    authlete: process.env["AUTHLETE_AUTHLETE"] ?? "",
  },
});

async function run() {
  const res = await joseObjectJoseVerifyApi(authlete, {
    serviceId: "<id>",
    requestBody: {
      jose: "eyJhbGciOiJFUzI1NiJ9.eyJleHAiOjE1NTk4MTE3NTAsImlzcyI6IjU3Mjk3NDA4ODY3In0K.csmdholMVcmjqHe59YWgLGNvm7I5Whp4phQCoGxyrlRGMnTgsfxtwyxBgMXQqEPD5q5k9FaEWNk37K8uAtSwrA",
      clockSkew: 100,
      clientIdentifier: "57297408867",
      signedByClient: true,
    },
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("joseObjectJoseVerifyApi failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.JoseVerifyApiRequest](../../models/operations/joseverifyapirequest.md)                                                                                             | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.JoseVerifyApiResponse](../../models/operations/joseverifyapiresponse.md)\>**

### Errors

| Error Type                                                        | Status Code                                                       | Content Type                                                      |
| ----------------------------------------------------------------- | ----------------------------------------------------------------- | ----------------------------------------------------------------- |
| errors.1api1infoGetResponses400Error                              | 400                                                               | application/json                                                  |
| errors.1api1infoGetResponses400ContentApplication1jsonSchemaError | 401, 403                                                          | application/json                                                  |
| errors.1api1infoGetResponses400ContentApplication1jsonSchemaError | 500                                                               | application/json                                                  |
| errors.AuthleteDefaultError                                       | 4XX, 5XX                                                          | \*/\*                                                             |

## joseVerifyApiForm

This API verifies a JOSE object.


### Example Usage

<!-- UsageSnippet language="typescript" operationID="jose_verify_api_form" method="post" path="/api/{serviceId}/jose/verify" -->
```typescript
import { Authlete } from "authlete-typescript-latest";

const authlete = new Authlete({
  security: {
    authlete: process.env["AUTHLETE_AUTHLETE"] ?? "",
  },
});

async function run() {
  const result = await authlete.joseObject.joseVerifyApiForm({
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
import { joseObjectJoseVerifyApiForm } from "authlete-typescript-latest/funcs/joseObjectJoseVerifyApiForm.js";

// Use `AuthleteCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const authlete = new AuthleteCore({
  security: {
    authlete: process.env["AUTHLETE_AUTHLETE"] ?? "",
  },
});

async function run() {
  const res = await joseObjectJoseVerifyApiForm(authlete, {
    serviceId: "<id>",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("joseObjectJoseVerifyApiForm failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.JoseVerifyApiFormRequest](../../models/operations/joseverifyapiformrequest.md)                                                                                     | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.JoseVerifyApiFormResponse](../../models/operations/joseverifyapiformresponse.md)\>**

### Errors

| Error Type                                                        | Status Code                                                       | Content Type                                                      |
| ----------------------------------------------------------------- | ----------------------------------------------------------------- | ----------------------------------------------------------------- |
| errors.1api1infoGetResponses400Error                              | 400                                                               | application/json                                                  |
| errors.1api1infoGetResponses400ContentApplication1jsonSchemaError | 401, 403                                                          | application/json                                                  |
| errors.1api1infoGetResponses400ContentApplication1jsonSchemaError | 500                                                               | application/json                                                  |
| errors.AuthleteDefaultError                                       | 4XX, 5XX                                                          | \*/\*                                                             |