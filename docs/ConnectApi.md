# ConnectApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**deleteConnectRevoke**](ConnectApi.md#deleteconnectrevoke) | **DELETE** /connect/revoke | Revoke a platform connection |
| [**postConnectExchange**](ConnectApi.md#postconnectexchangeoperation) | **POST** /connect/exchange | Exchange authorization code for API credentials |
| [**postConnectRevoke**](ConnectApi.md#postconnectrevokeoperation) | **POST** /connect/revoke | Revoke a platform connection (POST) |



## deleteConnectRevoke

> PostConnectRevoke200Response deleteConnectRevoke(postConnectRevokeRequest)

Revoke a platform connection

Revoke a connection between a platform and a Moosyl account. Deletes the connection\&#39;s API keys and webhook, so the platform loses access immediately.

### Example

```ts
import {
  Configuration,
  ConnectApi,
} from '@moosyl/sdk';
import type { DeleteConnectRevokeRequest } from '@moosyl/sdk';

async function example() {
  console.log("🚀 Testing @moosyl/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKey
    apiKey: "YOUR API KEY",
  });
  const api = new ConnectApi(config);

  const body = {
    // PostConnectRevokeRequest
    postConnectRevokeRequest: ...,
  } satisfies DeleteConnectRevokeRequest;

  try {
    const data = await api.deleteConnectRevoke(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **postConnectRevokeRequest** | [PostConnectRevokeRequest](PostConnectRevokeRequest.md) |  | |

### Return type

[**PostConnectRevoke200Response**](PostConnectRevoke200Response.md)

### Authorization

[ApiKey](../README.md#ApiKey)

### HTTP request headers

- **Content-Type**: `application/json`, `application/x-www-form-urlencoded`, `multipart/form-data`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Response for status 200 |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## postConnectExchange

> PostConnectExchange200Response postConnectExchange(postConnectExchangeRequest)

Exchange authorization code for API credentials

Exchange a short-lived authorization code (obtained from the /connect flow) for API keys dedicated to this connection, a webhook secret, and the connection ID used to revoke it. Connecting again replaces the keys and updates the same webhook.

### Example

```ts
import {
  Configuration,
  ConnectApi,
} from '@moosyl/sdk';
import type { PostConnectExchangeOperationRequest } from '@moosyl/sdk';

async function example() {
  console.log("🚀 Testing @moosyl/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKey
    apiKey: "YOUR API KEY",
  });
  const api = new ConnectApi(config);

  const body = {
    // PostConnectExchangeRequest
    postConnectExchangeRequest: ...,
  } satisfies PostConnectExchangeOperationRequest;

  try {
    const data = await api.postConnectExchange(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **postConnectExchangeRequest** | [PostConnectExchangeRequest](PostConnectExchangeRequest.md) |  | |

### Return type

[**PostConnectExchange200Response**](PostConnectExchange200Response.md)

### Authorization

[ApiKey](../README.md#ApiKey)

### HTTP request headers

- **Content-Type**: `application/json`, `application/x-www-form-urlencoded`, `multipart/form-data`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Response for status 200 |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## postConnectRevoke

> PostConnectRevoke200Response postConnectRevoke(postConnectRevokeRequest)

Revoke a platform connection (POST)

Revoke a connection between a platform and a Moosyl account. Deletes the connection\&#39;s API keys and webhook, so the platform loses access immediately.

### Example

```ts
import {
  Configuration,
  ConnectApi,
} from '@moosyl/sdk';
import type { PostConnectRevokeOperationRequest } from '@moosyl/sdk';

async function example() {
  console.log("🚀 Testing @moosyl/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKey
    apiKey: "YOUR API KEY",
  });
  const api = new ConnectApi(config);

  const body = {
    // PostConnectRevokeRequest
    postConnectRevokeRequest: ...,
  } satisfies PostConnectRevokeOperationRequest;

  try {
    const data = await api.postConnectRevoke(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **postConnectRevokeRequest** | [PostConnectRevokeRequest](PostConnectRevokeRequest.md) |  | |

### Return type

[**PostConnectRevoke200Response**](PostConnectRevoke200Response.md)

### Authorization

[ApiKey](../README.md#ApiKey)

### HTTP request headers

- **Content-Type**: `application/json`, `application/x-www-form-urlencoded`, `multipart/form-data`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Response for status 200 |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

