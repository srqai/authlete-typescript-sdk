# VerifiableCredentialIssuer
(*verifiableCredentialIssuer*)

## Overview

API endpoints for implementing and running a Verifiable Credential Issuer (VCI).

### Available Operations

* [vciMetadataApi](#vcimetadataapi) - /api/{serviceId}/vci/metadata API
* [vciMetadataApiForm](#vcimetadataapiform) - /api/{serviceId}/vci/metadata API
* [vciJwtissuerApi](#vcijwtissuerapi) - /api/{serviceId}/vci/jwtissuer API
* [vciJwtissuerApiForm](#vcijwtissuerapiform) - /api/{serviceId}/vci/jwtissuer API
* [vciJwksApi](#vcijwksapi) - /api/{serviceId}/vci/jwks API
* [vciJwksApiForm](#vcijwksapiform) - /api/{serviceId}/vci/jwks API
* [vciOfferCreateApi](#vcioffercreateapi) - /api/{serviceId}/vci/offer/create API
* [vciOfferCreateApiForm](#vcioffercreateapiform) - /api/{serviceId}/vci/offer/create API
* [vciOfferInfoApi](#vciofferinfoapi) - /api/{serviceId}/vci/offer/info API
* [vciOfferInfoApiForm](#vciofferinfoapiform) - /api/{serviceId}/vci/offer/info API
* [vciSingleParseApi](#vcisingleparseapi) - /api/{serviceId}/vci/single/parse API
* [vciSingleParseApiForm](#vcisingleparseapiform) - /api/{serviceId}/vci/single/parse API
* [vciSingleIssueApi](#vcisingleissueapi) - /api/{serviceId}/vci/single/issue API
* [vciBatchParseApi](#vcibatchparseapi) - /api/{serviceId}/vci/batch/parse API
* [vciBatchParseApiForm](#vcibatchparseapiform) - /api/{serviceId}/vci/batch/parse API
* [vciBatchIssueApi](#vcibatchissueapi) - /api/{serviceId}/vci/batch/issue API
* [vciDeferredParseApi](#vcideferredparseapi) - /api/{serviceId}/vci/deferred/parse API
* [vciDeferredParseApiForm](#vcideferredparseapiform) - /api/{serviceId}/vci/deferred/parse API
* [vciDeferredIssueApi](#vcideferredissueapi) - /api/{serviceId}/vci/deferred/issue API

## vciMetadataApi

/api/{serviceId}/vci/metadata API

### Example Usage

<!-- UsageSnippet language="typescript" operationID="vci_metadata_api" method="post" path="/api/{serviceId}/vci/metadata" -->
```typescript
import { Authlete } from "authlete-2";

const authlete = new Authlete({
  security: {
    authlete: process.env["AUTHLETE_AUTHLETE"] ?? "",
  },
});

async function run() {
  const result = await authlete.verifiableCredentialIssuer.vciMetadataApi({
    serviceId: "<id>",
    requestBody: {
      pretty: true,
    },
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { AuthleteCore } from "authlete-2/core.js";
import { verifiableCredentialIssuerVciMetadataApi } from "authlete-2/funcs/verifiableCredentialIssuerVciMetadataApi.js";

// Use `AuthleteCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const authlete = new AuthleteCore({
  security: {
    authlete: process.env["AUTHLETE_AUTHLETE"] ?? "",
  },
});

async function run() {
  const res = await verifiableCredentialIssuerVciMetadataApi(authlete, {
    serviceId: "<id>",
    requestBody: {
      pretty: true,
    },
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("verifiableCredentialIssuerVciMetadataApi failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.VciMetadataApiRequest](../../models/operations/vcimetadataapirequest.md)                                                                                           | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.VciMetadataApiResponse](../../models/operations/vcimetadataapiresponse.md)\>**

### Errors

| Error Type                  | Status Code                 | Content Type                |
| --------------------------- | --------------------------- | --------------------------- |
| errors.APIInfo400Error      | 400                         | application/json            |
| errors.APIInfo4002Error     | 401, 403                    | application/json            |
| errors.APIInfo4002Error     | 500                         | application/json            |
| errors.AuthleteDefaultError | 4XX, 5XX                    | \*/\*                       |

## vciMetadataApiForm

/api/{serviceId}/vci/metadata API

### Example Usage

<!-- UsageSnippet language="typescript" operationID="vci_metadata_api_form" method="post" path="/api/{serviceId}/vci/metadata" -->
```typescript
import { Authlete } from "authlete-2";

const authlete = new Authlete({
  security: {
    authlete: process.env["AUTHLETE_AUTHLETE"] ?? "",
  },
});

async function run() {
  const result = await authlete.verifiableCredentialIssuer.vciMetadataApiForm({
    serviceId: "<id>",
    apilBraceserviceIdRBraceVciMetadata: {},
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { AuthleteCore } from "authlete-2/core.js";
import { verifiableCredentialIssuerVciMetadataApiForm } from "authlete-2/funcs/verifiableCredentialIssuerVciMetadataApiForm.js";

// Use `AuthleteCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const authlete = new AuthleteCore({
  security: {
    authlete: process.env["AUTHLETE_AUTHLETE"] ?? "",
  },
});

async function run() {
  const res = await verifiableCredentialIssuerVciMetadataApiForm(authlete, {
    serviceId: "<id>",
    apilBraceserviceIdRBraceVciMetadata: {},
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("verifiableCredentialIssuerVciMetadataApiForm failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.VciMetadataApiFormRequest](../../models/operations/vcimetadataapiformrequest.md)                                                                                   | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.VciMetadataApiFormResponse](../../models/operations/vcimetadataapiformresponse.md)\>**

### Errors

| Error Type                  | Status Code                 | Content Type                |
| --------------------------- | --------------------------- | --------------------------- |
| errors.APIInfo400Error      | 400                         | application/json            |
| errors.APIInfo4002Error     | 401, 403                    | application/json            |
| errors.APIInfo4002Error     | 500                         | application/json            |
| errors.AuthleteDefaultError | 4XX, 5XX                    | \*/\*                       |

## vciJwtissuerApi

/api/{serviceId}/vci/jwtissuer API

### Example Usage

<!-- UsageSnippet language="typescript" operationID="vci_jwtissuer_api" method="post" path="/api/{serviceId}/vci/jwtissuer" -->
```typescript
import { Authlete } from "authlete-2";

const authlete = new Authlete({
  security: {
    authlete: process.env["AUTHLETE_AUTHLETE"] ?? "",
  },
});

async function run() {
  const result = await authlete.verifiableCredentialIssuer.vciJwtissuerApi({
    serviceId: "<id>",
    requestBody: {
      pretty: true,
    },
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { AuthleteCore } from "authlete-2/core.js";
import { verifiableCredentialIssuerVciJwtissuerApi } from "authlete-2/funcs/verifiableCredentialIssuerVciJwtissuerApi.js";

// Use `AuthleteCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const authlete = new AuthleteCore({
  security: {
    authlete: process.env["AUTHLETE_AUTHLETE"] ?? "",
  },
});

async function run() {
  const res = await verifiableCredentialIssuerVciJwtissuerApi(authlete, {
    serviceId: "<id>",
    requestBody: {
      pretty: true,
    },
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("verifiableCredentialIssuerVciJwtissuerApi failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.VciJwtissuerApiRequest](../../models/operations/vcijwtissuerapirequest.md)                                                                                         | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.VciJwtissuerApiResponse](../../models/operations/vcijwtissuerapiresponse.md)\>**

### Errors

| Error Type                  | Status Code                 | Content Type                |
| --------------------------- | --------------------------- | --------------------------- |
| errors.APIInfo400Error      | 400                         | application/json            |
| errors.APIInfo4002Error     | 401, 403                    | application/json            |
| errors.APIInfo4002Error     | 500                         | application/json            |
| errors.AuthleteDefaultError | 4XX, 5XX                    | \*/\*                       |

## vciJwtissuerApiForm

/api/{serviceId}/vci/jwtissuer API

### Example Usage

<!-- UsageSnippet language="typescript" operationID="vci_jwtissuer_api_form" method="post" path="/api/{serviceId}/vci/jwtissuer" -->
```typescript
import { Authlete } from "authlete-2";

const authlete = new Authlete({
  security: {
    authlete: process.env["AUTHLETE_AUTHLETE"] ?? "",
  },
});

async function run() {
  const result = await authlete.verifiableCredentialIssuer.vciJwtissuerApiForm({
    serviceId: "<id>",
    apilBraceserviceIdRBraceVciJwtissuer: {},
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { AuthleteCore } from "authlete-2/core.js";
import { verifiableCredentialIssuerVciJwtissuerApiForm } from "authlete-2/funcs/verifiableCredentialIssuerVciJwtissuerApiForm.js";

// Use `AuthleteCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const authlete = new AuthleteCore({
  security: {
    authlete: process.env["AUTHLETE_AUTHLETE"] ?? "",
  },
});

async function run() {
  const res = await verifiableCredentialIssuerVciJwtissuerApiForm(authlete, {
    serviceId: "<id>",
    apilBraceserviceIdRBraceVciJwtissuer: {},
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("verifiableCredentialIssuerVciJwtissuerApiForm failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.VciJwtissuerApiFormRequest](../../models/operations/vcijwtissuerapiformrequest.md)                                                                                 | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.VciJwtissuerApiFormResponse](../../models/operations/vcijwtissuerapiformresponse.md)\>**

### Errors

| Error Type                  | Status Code                 | Content Type                |
| --------------------------- | --------------------------- | --------------------------- |
| errors.APIInfo400Error      | 400                         | application/json            |
| errors.APIInfo4002Error     | 401, 403                    | application/json            |
| errors.APIInfo4002Error     | 500                         | application/json            |
| errors.AuthleteDefaultError | 4XX, 5XX                    | \*/\*                       |

## vciJwksApi

/api/{serviceId}/vci/jwks API

### Example Usage

<!-- UsageSnippet language="typescript" operationID="vci_jwks_api" method="post" path="/api/{serviceId}/vci/jwks" -->
```typescript
import { Authlete } from "authlete-2";

const authlete = new Authlete({
  security: {
    authlete: process.env["AUTHLETE_AUTHLETE"] ?? "",
  },
});

async function run() {
  const result = await authlete.verifiableCredentialIssuer.vciJwksApi({
    serviceId: "<id>",
    requestBody: {
      pretty: false,
    },
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { AuthleteCore } from "authlete-2/core.js";
import { verifiableCredentialIssuerVciJwksApi } from "authlete-2/funcs/verifiableCredentialIssuerVciJwksApi.js";

// Use `AuthleteCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const authlete = new AuthleteCore({
  security: {
    authlete: process.env["AUTHLETE_AUTHLETE"] ?? "",
  },
});

async function run() {
  const res = await verifiableCredentialIssuerVciJwksApi(authlete, {
    serviceId: "<id>",
    requestBody: {
      pretty: false,
    },
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("verifiableCredentialIssuerVciJwksApi failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.VciJwksApiRequest](../../models/operations/vcijwksapirequest.md)                                                                                                   | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.VciJwksApiResponse](../../models/operations/vcijwksapiresponse.md)\>**

### Errors

| Error Type                  | Status Code                 | Content Type                |
| --------------------------- | --------------------------- | --------------------------- |
| errors.APIInfo400Error      | 400                         | application/json            |
| errors.APIInfo4002Error     | 401, 403                    | application/json            |
| errors.APIInfo4002Error     | 500                         | application/json            |
| errors.AuthleteDefaultError | 4XX, 5XX                    | \*/\*                       |

## vciJwksApiForm

/api/{serviceId}/vci/jwks API

### Example Usage

<!-- UsageSnippet language="typescript" operationID="vci_jwks_api_form" method="post" path="/api/{serviceId}/vci/jwks" -->
```typescript
import { Authlete } from "authlete-2";

const authlete = new Authlete({
  security: {
    authlete: process.env["AUTHLETE_AUTHLETE"] ?? "",
  },
});

async function run() {
  const result = await authlete.verifiableCredentialIssuer.vciJwksApiForm({
    serviceId: "<id>",
    apilBraceserviceIdRBraceVciJwks: {},
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { AuthleteCore } from "authlete-2/core.js";
import { verifiableCredentialIssuerVciJwksApiForm } from "authlete-2/funcs/verifiableCredentialIssuerVciJwksApiForm.js";

// Use `AuthleteCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const authlete = new AuthleteCore({
  security: {
    authlete: process.env["AUTHLETE_AUTHLETE"] ?? "",
  },
});

async function run() {
  const res = await verifiableCredentialIssuerVciJwksApiForm(authlete, {
    serviceId: "<id>",
    apilBraceserviceIdRBraceVciJwks: {},
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("verifiableCredentialIssuerVciJwksApiForm failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.VciJwksApiFormRequest](../../models/operations/vcijwksapiformrequest.md)                                                                                           | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.VciJwksApiFormResponse](../../models/operations/vcijwksapiformresponse.md)\>**

### Errors

| Error Type                  | Status Code                 | Content Type                |
| --------------------------- | --------------------------- | --------------------------- |
| errors.APIInfo400Error      | 400                         | application/json            |
| errors.APIInfo4002Error     | 401, 403                    | application/json            |
| errors.APIInfo4002Error     | 500                         | application/json            |
| errors.AuthleteDefaultError | 4XX, 5XX                    | \*/\*                       |

## vciOfferCreateApi

/api/{serviceId}/vci/offer/create API

### Example Usage

<!-- UsageSnippet language="typescript" operationID="vci_offer_create_api" method="post" path="/api/{serviceId}/vci/offer/create" -->
```typescript
import { Authlete } from "authlete-2";

const authlete = new Authlete({
  security: {
    authlete: process.env["AUTHLETE_AUTHLETE"] ?? "",
  },
});

async function run() {
  const result = await authlete.verifiableCredentialIssuer.vciOfferCreateApi({
    serviceId: "<id>",
    requestBody: {},
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { AuthleteCore } from "authlete-2/core.js";
import { verifiableCredentialIssuerVciOfferCreateApi } from "authlete-2/funcs/verifiableCredentialIssuerVciOfferCreateApi.js";

// Use `AuthleteCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const authlete = new AuthleteCore({
  security: {
    authlete: process.env["AUTHLETE_AUTHLETE"] ?? "",
  },
});

async function run() {
  const res = await verifiableCredentialIssuerVciOfferCreateApi(authlete, {
    serviceId: "<id>",
    requestBody: {},
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("verifiableCredentialIssuerVciOfferCreateApi failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.VciOfferCreateApiRequest](../../models/operations/vcioffercreateapirequest.md)                                                                                     | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.VciOfferCreateApiResponse](../../models/operations/vcioffercreateapiresponse.md)\>**

### Errors

| Error Type                  | Status Code                 | Content Type                |
| --------------------------- | --------------------------- | --------------------------- |
| errors.APIInfo400Error      | 400                         | application/json            |
| errors.APIInfo4002Error     | 401, 403                    | application/json            |
| errors.APIInfo4002Error     | 500                         | application/json            |
| errors.AuthleteDefaultError | 4XX, 5XX                    | \*/\*                       |

## vciOfferCreateApiForm

/api/{serviceId}/vci/offer/create API

### Example Usage

<!-- UsageSnippet language="typescript" operationID="vci_offer_create_api_form" method="post" path="/api/{serviceId}/vci/offer/create" -->
```typescript
import { Authlete } from "authlete-2";

const authlete = new Authlete({
  security: {
    authlete: process.env["AUTHLETE_AUTHLETE"] ?? "",
  },
});

async function run() {
  const result = await authlete.verifiableCredentialIssuer.vciOfferCreateApiForm({
    serviceId: "<id>",
    apilBraceserviceIdRBraceVciOfferCreate: {},
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { AuthleteCore } from "authlete-2/core.js";
import { verifiableCredentialIssuerVciOfferCreateApiForm } from "authlete-2/funcs/verifiableCredentialIssuerVciOfferCreateApiForm.js";

// Use `AuthleteCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const authlete = new AuthleteCore({
  security: {
    authlete: process.env["AUTHLETE_AUTHLETE"] ?? "",
  },
});

async function run() {
  const res = await verifiableCredentialIssuerVciOfferCreateApiForm(authlete, {
    serviceId: "<id>",
    apilBraceserviceIdRBraceVciOfferCreate: {},
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("verifiableCredentialIssuerVciOfferCreateApiForm failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.VciOfferCreateApiFormRequest](../../models/operations/vcioffercreateapiformrequest.md)                                                                             | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.VciOfferCreateApiFormResponse](../../models/operations/vcioffercreateapiformresponse.md)\>**

### Errors

| Error Type                  | Status Code                 | Content Type                |
| --------------------------- | --------------------------- | --------------------------- |
| errors.APIInfo400Error      | 400                         | application/json            |
| errors.APIInfo4002Error     | 401, 403                    | application/json            |
| errors.APIInfo4002Error     | 500                         | application/json            |
| errors.AuthleteDefaultError | 4XX, 5XX                    | \*/\*                       |

## vciOfferInfoApi

/api/{serviceId}/vci/offer/info API

### Example Usage

<!-- UsageSnippet language="typescript" operationID="vci_offer_info_api" method="post" path="/api/{serviceId}/vci/offer/info" -->
```typescript
import { Authlete } from "authlete-2";

const authlete = new Authlete({
  security: {
    authlete: process.env["AUTHLETE_AUTHLETE"] ?? "",
  },
});

async function run() {
  const result = await authlete.verifiableCredentialIssuer.vciOfferInfoApi({
    serviceId: "<id>",
    requestBody: {},
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { AuthleteCore } from "authlete-2/core.js";
import { verifiableCredentialIssuerVciOfferInfoApi } from "authlete-2/funcs/verifiableCredentialIssuerVciOfferInfoApi.js";

// Use `AuthleteCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const authlete = new AuthleteCore({
  security: {
    authlete: process.env["AUTHLETE_AUTHLETE"] ?? "",
  },
});

async function run() {
  const res = await verifiableCredentialIssuerVciOfferInfoApi(authlete, {
    serviceId: "<id>",
    requestBody: {},
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("verifiableCredentialIssuerVciOfferInfoApi failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.VciOfferInfoApiRequest](../../models/operations/vciofferinfoapirequest.md)                                                                                         | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.VciOfferInfoApiResponse](../../models/operations/vciofferinfoapiresponse.md)\>**

### Errors

| Error Type                  | Status Code                 | Content Type                |
| --------------------------- | --------------------------- | --------------------------- |
| errors.APIInfo400Error      | 400                         | application/json            |
| errors.APIInfo4002Error     | 401, 403                    | application/json            |
| errors.APIInfo4002Error     | 500                         | application/json            |
| errors.AuthleteDefaultError | 4XX, 5XX                    | \*/\*                       |

## vciOfferInfoApiForm

/api/{serviceId}/vci/offer/info API

### Example Usage

<!-- UsageSnippet language="typescript" operationID="vci_offer_info_api_form" method="post" path="/api/{serviceId}/vci/offer/info" -->
```typescript
import { Authlete } from "authlete-2";

const authlete = new Authlete({
  security: {
    authlete: process.env["AUTHLETE_AUTHLETE"] ?? "",
  },
});

async function run() {
  const result = await authlete.verifiableCredentialIssuer.vciOfferInfoApiForm({
    serviceId: "<id>",
    apilBraceserviceIdRBraceVciOfferInfo: {},
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { AuthleteCore } from "authlete-2/core.js";
import { verifiableCredentialIssuerVciOfferInfoApiForm } from "authlete-2/funcs/verifiableCredentialIssuerVciOfferInfoApiForm.js";

// Use `AuthleteCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const authlete = new AuthleteCore({
  security: {
    authlete: process.env["AUTHLETE_AUTHLETE"] ?? "",
  },
});

async function run() {
  const res = await verifiableCredentialIssuerVciOfferInfoApiForm(authlete, {
    serviceId: "<id>",
    apilBraceserviceIdRBraceVciOfferInfo: {},
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("verifiableCredentialIssuerVciOfferInfoApiForm failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.VciOfferInfoApiFormRequest](../../models/operations/vciofferinfoapiformrequest.md)                                                                                 | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.VciOfferInfoApiFormResponse](../../models/operations/vciofferinfoapiformresponse.md)\>**

### Errors

| Error Type                  | Status Code                 | Content Type                |
| --------------------------- | --------------------------- | --------------------------- |
| errors.APIInfo400Error      | 400                         | application/json            |
| errors.APIInfo4002Error     | 401, 403                    | application/json            |
| errors.APIInfo4002Error     | 500                         | application/json            |
| errors.AuthleteDefaultError | 4XX, 5XX                    | \*/\*                       |

## vciSingleParseApi

/api/{serviceId}/vci/single/parse API

### Example Usage

<!-- UsageSnippet language="typescript" operationID="vci_single_parse_api" method="post" path="/api/{serviceId}/vci/single/parse" -->
```typescript
import { Authlete } from "authlete-2";

const authlete = new Authlete({
  security: {
    authlete: process.env["AUTHLETE_AUTHLETE"] ?? "",
  },
});

async function run() {
  const result = await authlete.verifiableCredentialIssuer.vciSingleParseApi({
    serviceId: "<id>",
    requestBody: {},
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { AuthleteCore } from "authlete-2/core.js";
import { verifiableCredentialIssuerVciSingleParseApi } from "authlete-2/funcs/verifiableCredentialIssuerVciSingleParseApi.js";

// Use `AuthleteCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const authlete = new AuthleteCore({
  security: {
    authlete: process.env["AUTHLETE_AUTHLETE"] ?? "",
  },
});

async function run() {
  const res = await verifiableCredentialIssuerVciSingleParseApi(authlete, {
    serviceId: "<id>",
    requestBody: {},
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("verifiableCredentialIssuerVciSingleParseApi failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.VciSingleParseApiRequest](../../models/operations/vcisingleparseapirequest.md)                                                                                     | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.VciSingleParseApiResponse](../../models/operations/vcisingleparseapiresponse.md)\>**

### Errors

| Error Type                  | Status Code                 | Content Type                |
| --------------------------- | --------------------------- | --------------------------- |
| errors.APIInfo400Error      | 400                         | application/json            |
| errors.APIInfo4002Error     | 401, 403                    | application/json            |
| errors.APIInfo4002Error     | 500                         | application/json            |
| errors.AuthleteDefaultError | 4XX, 5XX                    | \*/\*                       |

## vciSingleParseApiForm

/api/{serviceId}/vci/single/parse API

### Example Usage

<!-- UsageSnippet language="typescript" operationID="vci_single_parse_api_form" method="post" path="/api/{serviceId}/vci/single/parse" -->
```typescript
import { Authlete } from "authlete-2";

const authlete = new Authlete({
  security: {
    authlete: process.env["AUTHLETE_AUTHLETE"] ?? "",
  },
});

async function run() {
  const result = await authlete.verifiableCredentialIssuer.vciSingleParseApiForm({
    serviceId: "<id>",
    apilBraceserviceIdRBraceVciSingleParse: {},
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { AuthleteCore } from "authlete-2/core.js";
import { verifiableCredentialIssuerVciSingleParseApiForm } from "authlete-2/funcs/verifiableCredentialIssuerVciSingleParseApiForm.js";

// Use `AuthleteCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const authlete = new AuthleteCore({
  security: {
    authlete: process.env["AUTHLETE_AUTHLETE"] ?? "",
  },
});

async function run() {
  const res = await verifiableCredentialIssuerVciSingleParseApiForm(authlete, {
    serviceId: "<id>",
    apilBraceserviceIdRBraceVciSingleParse: {},
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("verifiableCredentialIssuerVciSingleParseApiForm failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.VciSingleParseApiFormRequest](../../models/operations/vcisingleparseapiformrequest.md)                                                                             | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.VciSingleParseApiFormResponse](../../models/operations/vcisingleparseapiformresponse.md)\>**

### Errors

| Error Type                  | Status Code                 | Content Type                |
| --------------------------- | --------------------------- | --------------------------- |
| errors.APIInfo400Error      | 400                         | application/json            |
| errors.APIInfo4002Error     | 401, 403                    | application/json            |
| errors.APIInfo4002Error     | 500                         | application/json            |
| errors.AuthleteDefaultError | 4XX, 5XX                    | \*/\*                       |

## vciSingleIssueApi

/api/{serviceId}/vci/single/issue API

### Example Usage

<!-- UsageSnippet language="typescript" operationID="vci_single_issue_api" method="post" path="/api/{serviceId}/vci/single/issue" -->
```typescript
import { Authlete } from "authlete-2";

const authlete = new Authlete({
  security: {
    authlete: process.env["AUTHLETE_AUTHLETE"] ?? "",
  },
});

async function run() {
  const result = await authlete.verifiableCredentialIssuer.vciSingleIssueApi({
    serviceId: "<id>",
    requestBody: {},
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { AuthleteCore } from "authlete-2/core.js";
import { verifiableCredentialIssuerVciSingleIssueApi } from "authlete-2/funcs/verifiableCredentialIssuerVciSingleIssueApi.js";

// Use `AuthleteCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const authlete = new AuthleteCore({
  security: {
    authlete: process.env["AUTHLETE_AUTHLETE"] ?? "",
  },
});

async function run() {
  const res = await verifiableCredentialIssuerVciSingleIssueApi(authlete, {
    serviceId: "<id>",
    requestBody: {},
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("verifiableCredentialIssuerVciSingleIssueApi failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.VciSingleIssueApiRequest](../../models/operations/vcisingleissueapirequest.md)                                                                                     | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.VciSingleIssueApiResponse](../../models/operations/vcisingleissueapiresponse.md)\>**

### Errors

| Error Type                  | Status Code                 | Content Type                |
| --------------------------- | --------------------------- | --------------------------- |
| errors.APIInfo400Error      | 400                         | application/json            |
| errors.APIInfo4002Error     | 401, 403                    | application/json            |
| errors.APIInfo4002Error     | 500                         | application/json            |
| errors.AuthleteDefaultError | 4XX, 5XX                    | \*/\*                       |

## vciBatchParseApi

/api/{serviceId}/vci/batch/parse API

### Example Usage

<!-- UsageSnippet language="typescript" operationID="vci_batch_parse_api" method="post" path="/api/{serviceId}/vci/batch/parse" -->
```typescript
import { Authlete } from "authlete-2";

const authlete = new Authlete({
  security: {
    authlete: process.env["AUTHLETE_AUTHLETE"] ?? "",
  },
});

async function run() {
  const result = await authlete.verifiableCredentialIssuer.vciBatchParseApi({
    serviceId: "<id>",
    requestBody: {},
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { AuthleteCore } from "authlete-2/core.js";
import { verifiableCredentialIssuerVciBatchParseApi } from "authlete-2/funcs/verifiableCredentialIssuerVciBatchParseApi.js";

// Use `AuthleteCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const authlete = new AuthleteCore({
  security: {
    authlete: process.env["AUTHLETE_AUTHLETE"] ?? "",
  },
});

async function run() {
  const res = await verifiableCredentialIssuerVciBatchParseApi(authlete, {
    serviceId: "<id>",
    requestBody: {},
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("verifiableCredentialIssuerVciBatchParseApi failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.VciBatchParseApiRequest](../../models/operations/vcibatchparseapirequest.md)                                                                                       | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.VciBatchParseApiResponse](../../models/operations/vcibatchparseapiresponse.md)\>**

### Errors

| Error Type                  | Status Code                 | Content Type                |
| --------------------------- | --------------------------- | --------------------------- |
| errors.APIInfo400Error      | 400                         | application/json            |
| errors.APIInfo4002Error     | 401, 403                    | application/json            |
| errors.APIInfo4002Error     | 500                         | application/json            |
| errors.AuthleteDefaultError | 4XX, 5XX                    | \*/\*                       |

## vciBatchParseApiForm

/api/{serviceId}/vci/batch/parse API

### Example Usage

<!-- UsageSnippet language="typescript" operationID="vci_batch_parse_api_form" method="post" path="/api/{serviceId}/vci/batch/parse" -->
```typescript
import { Authlete } from "authlete-2";

const authlete = new Authlete({
  security: {
    authlete: process.env["AUTHLETE_AUTHLETE"] ?? "",
  },
});

async function run() {
  const result = await authlete.verifiableCredentialIssuer.vciBatchParseApiForm({
    serviceId: "<id>",
    apilBraceserviceIdRBraceVciBatchParse: {},
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { AuthleteCore } from "authlete-2/core.js";
import { verifiableCredentialIssuerVciBatchParseApiForm } from "authlete-2/funcs/verifiableCredentialIssuerVciBatchParseApiForm.js";

// Use `AuthleteCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const authlete = new AuthleteCore({
  security: {
    authlete: process.env["AUTHLETE_AUTHLETE"] ?? "",
  },
});

async function run() {
  const res = await verifiableCredentialIssuerVciBatchParseApiForm(authlete, {
    serviceId: "<id>",
    apilBraceserviceIdRBraceVciBatchParse: {},
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("verifiableCredentialIssuerVciBatchParseApiForm failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.VciBatchParseApiFormRequest](../../models/operations/vcibatchparseapiformrequest.md)                                                                               | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.VciBatchParseApiFormResponse](../../models/operations/vcibatchparseapiformresponse.md)\>**

### Errors

| Error Type                  | Status Code                 | Content Type                |
| --------------------------- | --------------------------- | --------------------------- |
| errors.APIInfo400Error      | 400                         | application/json            |
| errors.APIInfo4002Error     | 401, 403                    | application/json            |
| errors.APIInfo4002Error     | 500                         | application/json            |
| errors.AuthleteDefaultError | 4XX, 5XX                    | \*/\*                       |

## vciBatchIssueApi

/api/{serviceId}/vci/batch/issue API

### Example Usage

<!-- UsageSnippet language="typescript" operationID="vci_batch_issue_api" method="post" path="/api/{serviceId}/vci/batch/issue" -->
```typescript
import { Authlete } from "authlete-2";

const authlete = new Authlete({
  security: {
    authlete: process.env["AUTHLETE_AUTHLETE"] ?? "",
  },
});

async function run() {
  const result = await authlete.verifiableCredentialIssuer.vciBatchIssueApi({
    serviceId: "<id>",
    requestBody: {},
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { AuthleteCore } from "authlete-2/core.js";
import { verifiableCredentialIssuerVciBatchIssueApi } from "authlete-2/funcs/verifiableCredentialIssuerVciBatchIssueApi.js";

// Use `AuthleteCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const authlete = new AuthleteCore({
  security: {
    authlete: process.env["AUTHLETE_AUTHLETE"] ?? "",
  },
});

async function run() {
  const res = await verifiableCredentialIssuerVciBatchIssueApi(authlete, {
    serviceId: "<id>",
    requestBody: {},
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("verifiableCredentialIssuerVciBatchIssueApi failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.VciBatchIssueApiRequest](../../models/operations/vcibatchissueapirequest.md)                                                                                       | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.VciBatchIssueApiResponse](../../models/operations/vcibatchissueapiresponse.md)\>**

### Errors

| Error Type                  | Status Code                 | Content Type                |
| --------------------------- | --------------------------- | --------------------------- |
| errors.APIInfo400Error      | 400                         | application/json            |
| errors.APIInfo4002Error     | 401, 403                    | application/json            |
| errors.APIInfo4002Error     | 500                         | application/json            |
| errors.AuthleteDefaultError | 4XX, 5XX                    | \*/\*                       |

## vciDeferredParseApi

/api/{serviceId}/vci/deferred/parse API

### Example Usage

<!-- UsageSnippet language="typescript" operationID="vci_deferred_parse_api" method="post" path="/api/{serviceId}/vci/deferred/parse" -->
```typescript
import { Authlete } from "authlete-2";

const authlete = new Authlete({
  security: {
    authlete: process.env["AUTHLETE_AUTHLETE"] ?? "",
  },
});

async function run() {
  const result = await authlete.verifiableCredentialIssuer.vciDeferredParseApi({
    serviceId: "<id>",
    requestBody: {},
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { AuthleteCore } from "authlete-2/core.js";
import { verifiableCredentialIssuerVciDeferredParseApi } from "authlete-2/funcs/verifiableCredentialIssuerVciDeferredParseApi.js";

// Use `AuthleteCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const authlete = new AuthleteCore({
  security: {
    authlete: process.env["AUTHLETE_AUTHLETE"] ?? "",
  },
});

async function run() {
  const res = await verifiableCredentialIssuerVciDeferredParseApi(authlete, {
    serviceId: "<id>",
    requestBody: {},
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("verifiableCredentialIssuerVciDeferredParseApi failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.VciDeferredParseApiRequest](../../models/operations/vcideferredparseapirequest.md)                                                                                 | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.VciDeferredParseApiResponse](../../models/operations/vcideferredparseapiresponse.md)\>**

### Errors

| Error Type                  | Status Code                 | Content Type                |
| --------------------------- | --------------------------- | --------------------------- |
| errors.APIInfo400Error      | 400                         | application/json            |
| errors.APIInfo4002Error     | 401, 403                    | application/json            |
| errors.APIInfo4002Error     | 500                         | application/json            |
| errors.AuthleteDefaultError | 4XX, 5XX                    | \*/\*                       |

## vciDeferredParseApiForm

/api/{serviceId}/vci/deferred/parse API

### Example Usage

<!-- UsageSnippet language="typescript" operationID="vci_deferred_parse_api_form" method="post" path="/api/{serviceId}/vci/deferred/parse" -->
```typescript
import { Authlete } from "authlete-2";

const authlete = new Authlete({
  security: {
    authlete: process.env["AUTHLETE_AUTHLETE"] ?? "",
  },
});

async function run() {
  const result = await authlete.verifiableCredentialIssuer.vciDeferredParseApiForm({
    serviceId: "<id>",
    apilBraceserviceIdRBraceVciDeferredParse: {},
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { AuthleteCore } from "authlete-2/core.js";
import { verifiableCredentialIssuerVciDeferredParseApiForm } from "authlete-2/funcs/verifiableCredentialIssuerVciDeferredParseApiForm.js";

// Use `AuthleteCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const authlete = new AuthleteCore({
  security: {
    authlete: process.env["AUTHLETE_AUTHLETE"] ?? "",
  },
});

async function run() {
  const res = await verifiableCredentialIssuerVciDeferredParseApiForm(authlete, {
    serviceId: "<id>",
    apilBraceserviceIdRBraceVciDeferredParse: {},
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("verifiableCredentialIssuerVciDeferredParseApiForm failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.VciDeferredParseApiFormRequest](../../models/operations/vcideferredparseapiformrequest.md)                                                                         | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.VciDeferredParseApiFormResponse](../../models/operations/vcideferredparseapiformresponse.md)\>**

### Errors

| Error Type                  | Status Code                 | Content Type                |
| --------------------------- | --------------------------- | --------------------------- |
| errors.APIInfo400Error      | 400                         | application/json            |
| errors.APIInfo4002Error     | 401, 403                    | application/json            |
| errors.APIInfo4002Error     | 500                         | application/json            |
| errors.AuthleteDefaultError | 4XX, 5XX                    | \*/\*                       |

## vciDeferredIssueApi

/api/{serviceId}/vci/deferred/issue API

### Example Usage

<!-- UsageSnippet language="typescript" operationID="vci_deferred_issue_api" method="post" path="/api/{serviceId}/vci/deferred/issue" -->
```typescript
import { Authlete } from "authlete-2";

const authlete = new Authlete({
  security: {
    authlete: process.env["AUTHLETE_AUTHLETE"] ?? "",
  },
});

async function run() {
  const result = await authlete.verifiableCredentialIssuer.vciDeferredIssueApi({
    serviceId: "<id>",
    requestBody: {},
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { AuthleteCore } from "authlete-2/core.js";
import { verifiableCredentialIssuerVciDeferredIssueApi } from "authlete-2/funcs/verifiableCredentialIssuerVciDeferredIssueApi.js";

// Use `AuthleteCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const authlete = new AuthleteCore({
  security: {
    authlete: process.env["AUTHLETE_AUTHLETE"] ?? "",
  },
});

async function run() {
  const res = await verifiableCredentialIssuerVciDeferredIssueApi(authlete, {
    serviceId: "<id>",
    requestBody: {},
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("verifiableCredentialIssuerVciDeferredIssueApi failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.VciDeferredIssueApiRequest](../../models/operations/vcideferredissueapirequest.md)                                                                                 | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.VciDeferredIssueApiResponse](../../models/operations/vcideferredissueapiresponse.md)\>**

### Errors

| Error Type                  | Status Code                 | Content Type                |
| --------------------------- | --------------------------- | --------------------------- |
| errors.APIInfo400Error      | 400                         | application/json            |
| errors.APIInfo4002Error     | 401, 403                    | application/json            |
| errors.APIInfo4002Error     | 500                         | application/json            |
| errors.AuthleteDefaultError | 4XX, 5XX                    | \*/\*                       |