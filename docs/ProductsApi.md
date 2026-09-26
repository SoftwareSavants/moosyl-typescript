# ProductsApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**getProducts**](ProductsApi.md#getproducts) | **GET** /products/ | List products or filter by id |
| [**getProductsById**](ProductsApi.md#getproductsbyid) | **GET** /products/{id} | Get product with prices |
| [**patchProductsById**](ProductsApi.md#patchproductsbyid) | **PATCH** /products/{id} | Update product |
| [**patchProductsByIdArchive**](ProductsApi.md#patchproductsbyidarchive) | **PATCH** /products/{id}/archive | Archive product |
| [**postProducts**](ProductsApi.md#postproducts) | **POST** /products/ | Create product |



## getProducts

> ProductList getProducts(id, page, limit)

List products or filter by id

### Example

```ts
import {
  Configuration,
  ProductsApi,
} from '@moosyl/sdk';
import type { GetProductsRequest } from '@moosyl/sdk';

async function example() {
  console.log("🚀 Testing @moosyl/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKey
    apiKey: "YOUR API KEY",
  });
  const api = new ProductsApi(config);

  const body = {
    // string (optional)
    id: id_example,
    // GetProductsPageParameter (optional)
    page: ...,
    // GetProductsPageParameter (optional)
    limit: ...,
  } satisfies GetProductsRequest;

  try {
    const data = await api.getProducts(body);
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
| **page** | [](.md) |  | [Optional] [Defaults to `undefined`] |
| **limit** | [](.md) |  | [Optional] [Defaults to `undefined`] |

### Return type

[**ProductList**](ProductList.md)

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


## getProductsById

> ProductGetWithPrices getProductsById(id)

Get product with prices

### Example

```ts
import {
  Configuration,
  ProductsApi,
} from '@moosyl/sdk';
import type { GetProductsByIdRequest } from '@moosyl/sdk';

async function example() {
  console.log("🚀 Testing @moosyl/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKey
    apiKey: "YOUR API KEY",
  });
  const api = new ProductsApi(config);

  const body = {
    // string
    id: id_example,
  } satisfies GetProductsByIdRequest;

  try {
    const data = await api.getProductsById(body);
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

[**ProductGetWithPrices**](ProductGetWithPrices.md)

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


## patchProductsById

> ProductGet patchProductsById(id, productUpdate)

Update product

### Example

```ts
import {
  Configuration,
  ProductsApi,
} from '@moosyl/sdk';
import type { PatchProductsByIdRequest } from '@moosyl/sdk';

async function example() {
  console.log("🚀 Testing @moosyl/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKey
    apiKey: "YOUR API KEY",
  });
  const api = new ProductsApi(config);

  const body = {
    // string
    id: id_example,
    // ProductUpdate
    productUpdate: ...,
  } satisfies PatchProductsByIdRequest;

  try {
    const data = await api.patchProductsById(body);
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
| **productUpdate** | [ProductUpdate](ProductUpdate.md) |  | |

### Return type

[**ProductGet**](ProductGet.md)

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


## patchProductsByIdArchive

> Success patchProductsByIdArchive(id)

Archive product

### Example

```ts
import {
  Configuration,
  ProductsApi,
} from '@moosyl/sdk';
import type { PatchProductsByIdArchiveRequest } from '@moosyl/sdk';

async function example() {
  console.log("🚀 Testing @moosyl/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKey
    apiKey: "YOUR API KEY",
  });
  const api = new ProductsApi(config);

  const body = {
    // string
    id: id_example,
  } satisfies PatchProductsByIdArchiveRequest;

  try {
    const data = await api.patchProductsByIdArchive(body);
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

[**Success**](Success.md)

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


## postProducts

> ProductGet postProducts(productCreate)

Create product

### Example

```ts
import {
  Configuration,
  ProductsApi,
} from '@moosyl/sdk';
import type { PostProductsRequest } from '@moosyl/sdk';

async function example() {
  console.log("🚀 Testing @moosyl/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKey
    apiKey: "YOUR API KEY",
  });
  const api = new ProductsApi(config);

  const body = {
    // ProductCreate
    productCreate: ...,
  } satisfies PostProductsRequest;

  try {
    const data = await api.postProducts(body);
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
| **productCreate** | [ProductCreate](ProductCreate.md) |  | |

### Return type

[**ProductGet**](ProductGet.md)

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

