# OrganizationApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**getOrganizationById**](OrganizationApi.md#getorganizationbyid) | **GET** /organization/{id} | Get organization details |



## getOrganizationById

> GetOrganizationById200Response getOrganizationById(id)

Get organization details

Retrieve organization information. Requires secret API key.

### Example

```ts
import {
  Configuration,
  OrganizationApi,
} from '@moosyl/sdk';
import type { GetOrganizationByIdRequest } from '@moosyl/sdk';

async function example() {
  console.log("🚀 Testing @moosyl/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKey
    apiKey: "YOUR API KEY",
  });
  const api = new OrganizationApi(config);

  const body = {
    // string
    id: id_example,
  } satisfies GetOrganizationByIdRequest;

  try {
    const data = await api.getOrganizationById(body);
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
| **id** | `string` |  | [Defaults to `undefined`] |

### Return type

[**GetOrganizationById200Response**](GetOrganizationById200Response.md)

### Authorization

[ApiKey](../README.md#ApiKey)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Response for status 200 |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

