# SubscriptionsApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**getSubscriptions**](SubscriptionsApi.md#getsubscriptions) | **GET** /subscriptions/ | List subscriptions |
| [**getSubscriptionsByExternalUserByExternalUserId**](SubscriptionsApi.md#getsubscriptionsbyexternaluserbyexternaluserid) | **GET** /subscriptions/by-external-user/{externalUserId} | Get subscription by external user |
| [**getSubscriptionsById**](SubscriptionsApi.md#getsubscriptionsbyid) | **GET** /subscriptions/{id} | Get subscription |
| [**postSubscriptions**](SubscriptionsApi.md#postsubscriptions) | **POST** /subscriptions/ | Create subscription |
| [**postSubscriptionsByExternalUser**](SubscriptionsApi.md#postsubscriptionsbyexternaluser) | **POST** /subscriptions/by-external-user | Create subscription by external user |
| [**postSubscriptionsByIdCancel**](SubscriptionsApi.md#postsubscriptionsbyidcancel) | **POST** /subscriptions/{id}/cancel | Cancel subscription |



## getSubscriptions

> SubscriptionList getSubscriptions(status, page, limit)

List subscriptions

### Example

```ts
import {
  Configuration,
  SubscriptionsApi,
} from '@moosyl/sdk';
import type { GetSubscriptionsRequest } from '@moosyl/sdk';

async function example() {
  console.log("🚀 Testing @moosyl/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKey
    apiKey: "YOUR API KEY",
  });
  const api = new SubscriptionsApi(config);

  const body = {
    // 'trialing' | 'active' | 'past_due' | 'paused' | 'cancelled' | 'expired' | 'pending_cancellation' (optional)
    status: status_example,
    // GetProductsPageParameter (optional)
    page: ...,
    // GetProductsPageParameter (optional)
    limit: ...,
  } satisfies GetSubscriptionsRequest;

  try {
    const data = await api.getSubscriptions(body);
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
| **status** | `trialing`, `active`, `past_due`, `paused`, `cancelled`, `expired`, `pending_cancellation` |  | [Optional] [Defaults to `undefined`] [Enum: trialing, active, past_due, paused, cancelled, expired, pending_cancellation] |
| **page** | [](.md) |  | [Optional] [Defaults to `undefined`] |
| **limit** | [](.md) |  | [Optional] [Defaults to `undefined`] |

### Return type

[**SubscriptionList**](SubscriptionList.md)

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


## getSubscriptionsByExternalUserByExternalUserId

> SubscriptionGet getSubscriptionsByExternalUserByExternalUserId(externalUserId)

Get subscription by external user

### Example

```ts
import {
  Configuration,
  SubscriptionsApi,
} from '@moosyl/sdk';
import type { GetSubscriptionsByExternalUserByExternalUserIdRequest } from '@moosyl/sdk';

async function example() {
  console.log("🚀 Testing @moosyl/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKey
    apiKey: "YOUR API KEY",
  });
  const api = new SubscriptionsApi(config);

  const body = {
    // string
    externalUserId: externalUserId_example,
  } satisfies GetSubscriptionsByExternalUserByExternalUserIdRequest;

  try {
    const data = await api.getSubscriptionsByExternalUserByExternalUserId(body);
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
| **externalUserId** | `string` |  | [Defaults to `undefined`] |

### Return type

[**SubscriptionGet**](SubscriptionGet.md)

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


## getSubscriptionsById

> SubscriptionGet getSubscriptionsById(id)

Get subscription

### Example

```ts
import {
  Configuration,
  SubscriptionsApi,
} from '@moosyl/sdk';
import type { GetSubscriptionsByIdRequest } from '@moosyl/sdk';

async function example() {
  console.log("🚀 Testing @moosyl/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKey
    apiKey: "YOUR API KEY",
  });
  const api = new SubscriptionsApi(config);

  const body = {
    // string
    id: id_example,
  } satisfies GetSubscriptionsByIdRequest;

  try {
    const data = await api.getSubscriptionsById(body);
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

[**SubscriptionGet**](SubscriptionGet.md)

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


## postSubscriptions

> SubscriptionGet postSubscriptions(subscriptionCreate)

Create subscription

### Example

```ts
import {
  Configuration,
  SubscriptionsApi,
} from '@moosyl/sdk';
import type { PostSubscriptionsRequest } from '@moosyl/sdk';

async function example() {
  console.log("🚀 Testing @moosyl/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKey
    apiKey: "YOUR API KEY",
  });
  const api = new SubscriptionsApi(config);

  const body = {
    // SubscriptionCreate
    subscriptionCreate: ...,
  } satisfies PostSubscriptionsRequest;

  try {
    const data = await api.postSubscriptions(body);
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
| **subscriptionCreate** | [SubscriptionCreate](SubscriptionCreate.md) |  | |

### Return type

[**SubscriptionGet**](SubscriptionGet.md)

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


## postSubscriptionsByExternalUser

> SubscriptionGet postSubscriptionsByExternalUser(subscriptionCreateByExternalUser)

Create subscription by external user

### Example

```ts
import {
  Configuration,
  SubscriptionsApi,
} from '@moosyl/sdk';
import type { PostSubscriptionsByExternalUserRequest } from '@moosyl/sdk';

async function example() {
  console.log("🚀 Testing @moosyl/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKey
    apiKey: "YOUR API KEY",
  });
  const api = new SubscriptionsApi(config);

  const body = {
    // SubscriptionCreateByExternalUser
    subscriptionCreateByExternalUser: ...,
  } satisfies PostSubscriptionsByExternalUserRequest;

  try {
    const data = await api.postSubscriptionsByExternalUser(body);
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
| **subscriptionCreateByExternalUser** | [SubscriptionCreateByExternalUser](SubscriptionCreateByExternalUser.md) |  | |

### Return type

[**SubscriptionGet**](SubscriptionGet.md)

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


## postSubscriptionsByIdCancel

> SubscriptionGet postSubscriptionsByIdCancel(id)

Cancel subscription

### Example

```ts
import {
  Configuration,
  SubscriptionsApi,
} from '@moosyl/sdk';
import type { PostSubscriptionsByIdCancelRequest } from '@moosyl/sdk';

async function example() {
  console.log("🚀 Testing @moosyl/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKey
    apiKey: "YOUR API KEY",
  });
  const api = new SubscriptionsApi(config);

  const body = {
    // string
    id: id_example,
  } satisfies PostSubscriptionsByIdCancelRequest;

  try {
    const data = await api.postSubscriptionsByIdCancel(body);
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

[**SubscriptionGet**](SubscriptionGet.md)

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

