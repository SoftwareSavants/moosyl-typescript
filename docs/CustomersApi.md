# CustomersApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**getCustomers**](CustomersApi.md#getcustomers) | **GET** /customers/ | List customers or filter by id/external user |
| [**patchCustomersById**](CustomersApi.md#patchcustomersbyid) | **PATCH** /customers/{id} | Update customer |
| [**postCustomers**](CustomersApi.md#postcustomers) | **POST** /customers/ | Create customer |



## getCustomers

> CustomerList getCustomers(id, externalUserId, page, limit)

List customers or filter by id/external user

### Example

```ts
import {
  Configuration,
  CustomersApi,
} from '@moosyl/sdk';
import type { GetCustomersRequest } from '@moosyl/sdk';

async function example() {
  console.log("🚀 Testing @moosyl/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKey
    apiKey: "YOUR API KEY",
  });
  const api = new CustomersApi(config);

  const body = {
    // string (optional)
    id: id_example,
    // string (optional)
    externalUserId: externalUserId_example,
    // GetProductsPageParameter (optional)
    page: ...,
    // GetProductsPageParameter (optional)
    limit: ...,
  } satisfies GetCustomersRequest;

  try {
    const data = await api.getCustomers(body);
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
| **id** | `string` |  | [Optional] [Defaults to `undefined`] |
| **externalUserId** | `string` |  | [Optional] [Defaults to `undefined`] |
| **page** | [](.md) |  | [Optional] [Defaults to `undefined`] |
| **limit** | [](.md) |  | [Optional] [Defaults to `undefined`] |

### Return type

[**CustomerList**](CustomerList.md)

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


## patchCustomersById

> CustomerGet patchCustomersById(id, customerUpdate)

Update customer

### Example

```ts
import {
  Configuration,
  CustomersApi,
} from '@moosyl/sdk';
import type { PatchCustomersByIdRequest } from '@moosyl/sdk';

async function example() {
  console.log("🚀 Testing @moosyl/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKey
    apiKey: "YOUR API KEY",
  });
  const api = new CustomersApi(config);

  const body = {
    // string
    id: id_example,
    // CustomerUpdate
    customerUpdate: ...,
  } satisfies PatchCustomersByIdRequest;

  try {
    const data = await api.patchCustomersById(body);
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
| **customerUpdate** | [CustomerUpdate](CustomerUpdate.md) |  | |

### Return type

[**CustomerGet**](CustomerGet.md)

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


## postCustomers

> CustomerGet postCustomers(customerCreate)

Create customer

### Example

```ts
import {
  Configuration,
  CustomersApi,
} from '@moosyl/sdk';
import type { PostCustomersRequest } from '@moosyl/sdk';

async function example() {
  console.log("🚀 Testing @moosyl/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKey
    apiKey: "YOUR API KEY",
  });
  const api = new CustomersApi(config);

  const body = {
    // CustomerCreate
    customerCreate: ...,
  } satisfies PostCustomersRequest;

  try {
    const data = await api.postCustomers(body);
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
| **customerCreate** | [CustomerCreate](CustomerCreate.md) |  | |

### Return type

[**CustomerGet**](CustomerGet.md)

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

