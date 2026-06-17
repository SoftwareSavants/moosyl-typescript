# CronApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**postCronBillingCycle**](CronApi.md#postcronbillingcycle) | **POST** /cron/billing-cycle | Process billing cycles |
| [**postCronExpireSubscriptions**](CronApi.md#postcronexpiresubscriptions) | **POST** /cron/expire-subscriptions | Process due cancellations and expirations |



## postCronBillingCycle

> CronResult postCronBillingCycle()

Process billing cycles

### Example

```ts
import {
  Configuration,
  CronApi,
} from '@moosyl/sdk';
import type { PostCronBillingCycleRequest } from '@moosyl/sdk';

async function example() {
  console.log("🚀 Testing @moosyl/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKey
    apiKey: "YOUR API KEY",
  });
  const api = new CronApi(config);

  try {
    const data = await api.postCronBillingCycle();
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

[**CronResult**](CronResult.md)

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


## postCronExpireSubscriptions

> CronResult postCronExpireSubscriptions()

Process due cancellations and expirations

### Example

```ts
import {
  Configuration,
  CronApi,
} from '@moosyl/sdk';
import type { PostCronExpireSubscriptionsRequest } from '@moosyl/sdk';

async function example() {
  console.log("🚀 Testing @moosyl/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKey
    apiKey: "YOUR API KEY",
  });
  const api = new CronApi(config);

  try {
    const data = await api.postCronExpireSubscriptions();
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

[**CronResult**](CronResult.md)

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

