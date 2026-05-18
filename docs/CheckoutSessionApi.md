# CheckoutSessionApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**getCheckoutSessionPublicById**](CheckoutSessionApi.md#getcheckoutsessionpublicbyid) | **GET** /checkout-session/public/{id} | Get public checkout session |
| [**postCheckoutSession**](CheckoutSessionApi.md#postcheckoutsession) | **POST** /checkout-session | Create checkout session |
| [**postCheckoutSessionPublicByIdPay**](CheckoutSessionApi.md#postcheckoutsessionpublicbyidpay) | **POST** /checkout-session/public/{id}/pay | Pay public checkout session |
| [**postCheckoutSessionPublicByIdSwitchMethod**](CheckoutSessionApi.md#postcheckoutsessionpublicbyidswitchmethod) | **POST** /checkout-session/public/{id}/switch-method | Switch public checkout method |



## getCheckoutSessionPublicById

> CheckoutSessionGet getCheckoutSessionPublicById(id)

Get public checkout session

Get checkout session details without an API key.

### Example

```ts
import {
  Configuration,
  CheckoutSessionApi,
} from '@moosyl/sdk';
import type { GetCheckoutSessionPublicByIdRequest } from '@moosyl/sdk';

async function example() {
  console.log("🚀 Testing @moosyl/sdk SDK...");
  const api = new CheckoutSessionApi();

  const body = {
    // string
    id: id_example,
  } satisfies GetCheckoutSessionPublicByIdRequest;

  try {
    const data = await api.getCheckoutSessionPublicById(body);
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

[**CheckoutSessionGet**](CheckoutSessionGet.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Response for status 200 |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## postCheckoutSession

> CheckoutSessionCreate postCheckoutSession(checkoutSessionCreateBody)

Create checkout session

Create a hosted checkout session from paymentRequestId, or from transactionId (optionally creating the payment request when amount is provided).

### Example

```ts
import {
  Configuration,
  CheckoutSessionApi,
} from '@moosyl/sdk';
import type { PostCheckoutSessionRequest } from '@moosyl/sdk';

async function example() {
  console.log("🚀 Testing @moosyl/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKey
    apiKey: "YOUR API KEY",
  });
  const api = new CheckoutSessionApi(config);

  const body = {
    // CheckoutSessionCreateBody
    checkoutSessionCreateBody: ...,
  } satisfies PostCheckoutSessionRequest;

  try {
    const data = await api.postCheckoutSession(body);
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
| **checkoutSessionCreateBody** | [CheckoutSessionCreateBody](CheckoutSessionCreateBody.md) |  | |

### Return type

[**CheckoutSessionCreate**](CheckoutSessionCreate.md)

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


## postCheckoutSessionPublicByIdPay

> PostCheckoutSessionPublicByIdPay200Response postCheckoutSessionPublicByIdPay(id, checkoutSessionPayBody)

Pay public checkout session

Create payment for a checkout session without requiring API key in the client.

### Example

```ts
import {
  Configuration,
  CheckoutSessionApi,
} from '@moosyl/sdk';
import type { PostCheckoutSessionPublicByIdPayRequest } from '@moosyl/sdk';

async function example() {
  console.log("🚀 Testing @moosyl/sdk SDK...");
  const api = new CheckoutSessionApi();

  const body = {
    // string
    id: id_example,
    // CheckoutSessionPayBody
    checkoutSessionPayBody: ...,
  } satisfies PostCheckoutSessionPublicByIdPayRequest;

  try {
    const data = await api.postCheckoutSessionPublicByIdPay(body);
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
| **checkoutSessionPayBody** | [CheckoutSessionPayBody](CheckoutSessionPayBody.md) |  | |

### Return type

[**PostCheckoutSessionPublicByIdPay200Response**](PostCheckoutSessionPublicByIdPay200Response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: `application/json`, `application/x-www-form-urlencoded`, `multipart/form-data`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Response for status 200 |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## postCheckoutSessionPublicByIdSwitchMethod

> CheckoutSessionSwitchMethod postCheckoutSessionPublicByIdSwitchMethod(id, checkoutSessionSelectMethodBody)

Switch public checkout method

Switch checkout method and cancel the latest pending payment when present.

### Example

```ts
import {
  Configuration,
  CheckoutSessionApi,
} from '@moosyl/sdk';
import type { PostCheckoutSessionPublicByIdSwitchMethodRequest } from '@moosyl/sdk';

async function example() {
  console.log("🚀 Testing @moosyl/sdk SDK...");
  const api = new CheckoutSessionApi();

  const body = {
    // string
    id: id_example,
    // CheckoutSessionSelectMethodBody
    checkoutSessionSelectMethodBody: ...,
  } satisfies PostCheckoutSessionPublicByIdSwitchMethodRequest;

  try {
    const data = await api.postCheckoutSessionPublicByIdSwitchMethod(body);
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
| **checkoutSessionSelectMethodBody** | [CheckoutSessionSelectMethodBody](CheckoutSessionSelectMethodBody.md) |  | |

### Return type

[**CheckoutSessionSwitchMethod**](CheckoutSessionSwitchMethod.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: `application/json`, `application/x-www-form-urlencoded`, `multipart/form-data`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Response for status 200 |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

