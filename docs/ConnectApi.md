# ConnectApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**deleteConnectRevoke**](ConnectApi.md#deleteconnectrevokeoperation) | **DELETE** /connect/revoke | Revoke a platform connection |
| [**postConnectExchange**](ConnectApi.md#postconnectexchangeoperation) | **POST** /connect/exchange | Exchange authorization code for API credentials |



## deleteConnectRevoke

> DeleteConnectRevoke200Response deleteConnectRevoke(deleteConnectRevokeRequest)

Revoke a platform connection

Revoke a previously authorized connection between a platform and a Moosyl account.

### Example

```ts
import {
  Configuration,
  ConnectApi,
} from '@moosyl/sdk';
import type { DeleteConnectRevokeOperationRequest } from '@moosyl/sdk';

async function example() {
  console.log("🚀 Testing @moosyl/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKey
    apiKey: "YOUR API KEY",
  });
  const api = new ConnectApi(config);

  const body = {
    // DeleteConnectRevokeRequest
    deleteConnectRevokeRequest: ...,
  } satisfies DeleteConnectRevokeOperationRequest;

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
| **deleteConnectRevokeRequest** | [DeleteConnectRevokeRequest](DeleteConnectRevokeRequest.md) |  | |

### Return type

[**DeleteConnectRevoke200Response**](DeleteConnectRevoke200Response.md)

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

Exchange a short-lived authorization code (obtained from the /connect flow) for the user\&#39;s publishable key, secret key, and webhook secret. A webhook will be created using the provided endpoints.

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

