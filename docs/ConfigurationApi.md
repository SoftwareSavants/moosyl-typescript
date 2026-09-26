# ConfigurationApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**getConfiguration**](ConfigurationApi.md#getconfiguration) | **GET** /configuration | List configurations |
| [**getConfigurationById**](ConfigurationApi.md#getconfigurationbyid) | **GET** /configuration/{id} | Get configuration |



## getConfiguration

> ConfigurationList getConfiguration()

List configurations

Retrieve all configurations for the current environment

### Example

```ts
import {
  Configuration,
  ConfigurationApi,
} from '@moosyl/sdk';
import type { GetConfigurationRequest } from '@moosyl/sdk';

async function example() {
  console.log("🚀 Testing @moosyl/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKey
    apiKey: "YOUR API KEY",
  });
  const api = new ConfigurationApi(config);

  try {
    const data = await api.getConfiguration();
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**ConfigurationList**](ConfigurationList.md)

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


## getConfigurationById

> ConfigurationGet getConfigurationById(id)

Get configuration

Retrieve a specific configuration by ID. Requires secret API key.

### Example

```ts
import {
  Configuration,
  ConfigurationApi,
} from '@moosyl/sdk';
import type { GetConfigurationByIdRequest } from '@moosyl/sdk';

async function example() {
  console.log("🚀 Testing @moosyl/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKey
    apiKey: "YOUR API KEY",
  });
  const api = new ConfigurationApi(config);

  const body = {
    // string
    id: id_example,
  } satisfies GetConfigurationByIdRequest;

  try {
    const data = await api.getConfigurationById(body);
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

[**ConfigurationGet**](ConfigurationGet.md)

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

