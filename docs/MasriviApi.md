# MasriviApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**postMasriviInitiate**](MasriviApi.md#postmasriviinitiateoperation) | **POST** /masrivi/initiate | Initiate Masrivi payment |



## postMasriviInitiate

> PostMasriviInitiate200Response postMasriviInitiate(postMasriviInitiateRequest)

Initiate Masrivi payment

Creates a pending payment and returns form data to redirect customer to Masrivi payment page.

### Example

```ts
import {
  Configuration,
  MasriviApi,
} from '@moosyl/sdk';
import type { PostMasriviInitiateOperationRequest } from '@moosyl/sdk';

async function example() {
  console.log("🚀 Testing @moosyl/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKey
    apiKey: "YOUR API KEY",
  });
  const api = new MasriviApi(config);

  const body = {
    // PostMasriviInitiateRequest
    postMasriviInitiateRequest: ...,
  } satisfies PostMasriviInitiateOperationRequest;

  try {
    const data = await api.postMasriviInitiate(body);
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
| **postMasriviInitiateRequest** | [PostMasriviInitiateRequest](PostMasriviInitiateRequest.md) |  | |

### Return type

[**PostMasriviInitiate200Response**](PostMasriviInitiate200Response.md)

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

