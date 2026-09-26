# PricesApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**getPricesById**](PricesApi.md#getpricesbyid) | **GET** /prices/{id} | Get price |
| [**patchPricesById**](PricesApi.md#patchpricesbyid) | **PATCH** /prices/{id} | Update price |
| [**patchPricesByIdArchive**](PricesApi.md#patchpricesbyidarchive) | **PATCH** /prices/{id}/archive | Archive price |
| [**postPrices**](PricesApi.md#postprices) | **POST** /prices/ | Create price |



## getPricesById

> PriceGet getPricesById(id)

Get price

### Example

```ts
import {
  Configuration,
  PricesApi,
} from '@moosyl/sdk';
import type { GetPricesByIdRequest } from '@moosyl/sdk';

async function example() {
  console.log("🚀 Testing @moosyl/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKey
    apiKey: "YOUR API KEY",
  });
  const api = new PricesApi(config);

  const body = {
    // string
    id: id_example,
  } satisfies GetPricesByIdRequest;

  try {
    const data = await api.getPricesById(body);
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

[**PriceGet**](PriceGet.md)

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


## patchPricesById

> PriceGet patchPricesById(id, priceUpdate)

Update price

### Example

```ts
import {
  Configuration,
  PricesApi,
} from '@moosyl/sdk';
import type { PatchPricesByIdRequest } from '@moosyl/sdk';

async function example() {
  console.log("🚀 Testing @moosyl/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKey
    apiKey: "YOUR API KEY",
  });
  const api = new PricesApi(config);

  const body = {
    // string
    id: id_example,
    // PriceUpdate
    priceUpdate: ...,
  } satisfies PatchPricesByIdRequest;

  try {
    const data = await api.patchPricesById(body);
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
| **priceUpdate** | [PriceUpdate](PriceUpdate.md) |  | |

### Return type

[**PriceGet**](PriceGet.md)

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


## patchPricesByIdArchive

> Success patchPricesByIdArchive(id)

Archive price

### Example

```ts
import {
  Configuration,
  PricesApi,
} from '@moosyl/sdk';
import type { PatchPricesByIdArchiveRequest } from '@moosyl/sdk';

async function example() {
  console.log("🚀 Testing @moosyl/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKey
    apiKey: "YOUR API KEY",
  });
  const api = new PricesApi(config);

  const body = {
    // string
    id: id_example,
  } satisfies PatchPricesByIdArchiveRequest;

  try {
    const data = await api.patchPricesByIdArchive(body);
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


## postPrices

> PriceGet postPrices(priceCreate)

Create price

### Example

```ts
import {
  Configuration,
  PricesApi,
} from '@moosyl/sdk';
import type { PostPricesRequest } from '@moosyl/sdk';

async function example() {
  console.log("🚀 Testing @moosyl/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKey
    apiKey: "YOUR API KEY",
  });
  const api = new PricesApi(config);

  const body = {
    // PriceCreate
    priceCreate: ...,
  } satisfies PostPricesRequest;

  try {
    const data = await api.postPrices(body);
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
| **priceCreate** | [PriceCreate](PriceCreate.md) |  | |

### Return type

[**PriceGet**](PriceGet.md)

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

