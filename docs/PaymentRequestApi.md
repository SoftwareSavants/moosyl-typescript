# PaymentRequestApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**getPaymentRequestById**](PaymentRequestApi.md#getpaymentrequestbyid) | **GET** /payment-request/{id} | Get payment request |
| [**getPaymentRequestByTransactionByTransactionId**](PaymentRequestApi.md#getpaymentrequestbytransactionbytransactionid) | **GET** /payment-request/by-transaction/{transactionId} | Get payment request by transaction ID |
| [**patchPaymentRequestByTransactionIdRefreshStatus**](PaymentRequestApi.md#patchpaymentrequestbytransactionidrefreshstatus) | **PATCH** /payment-request/{transactionId}/refresh-status | Refresh payment request status |
| [**postPaymentRequest**](PaymentRequestApi.md#postpaymentrequest) | **POST** /payment-request | Create payment request |



## getPaymentRequestById

> PaymentRequestGet getPaymentRequestById(id)

Get payment request

Retrieve a payment request by ID

### Example

```ts
import {
  Configuration,
  PaymentRequestApi,
} from '@moosyl/sdk';
import type { GetPaymentRequestByIdRequest } from '@moosyl/sdk';

async function example() {
  console.log("🚀 Testing @moosyl/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKey
    apiKey: "YOUR API KEY",
  });
  const api = new PaymentRequestApi(config);

  const body = {
    // string
    id: id_example,
  } satisfies GetPaymentRequestByIdRequest;

  try {
    const data = await api.getPaymentRequestById(body);
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

[**PaymentRequestGet**](PaymentRequestGet.md)

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


## getPaymentRequestByTransactionByTransactionId

> PaymentRequestGet getPaymentRequestByTransactionByTransactionId(transactionId)

Get payment request by transaction ID

Retrieve a payment request by transaction ID

### Example

```ts
import {
  Configuration,
  PaymentRequestApi,
} from '@moosyl/sdk';
import type { GetPaymentRequestByTransactionByTransactionIdRequest } from '@moosyl/sdk';

async function example() {
  console.log("🚀 Testing @moosyl/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKey
    apiKey: "YOUR API KEY",
  });
  const api = new PaymentRequestApi(config);

  const body = {
    // string
    transactionId: transactionId_example,
  } satisfies GetPaymentRequestByTransactionByTransactionIdRequest;

  try {
    const data = await api.getPaymentRequestByTransactionByTransactionId(body);
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
| **transactionId** | `string` |  | [Defaults to `undefined`] |

### Return type

[**PaymentRequestGet**](PaymentRequestGet.md)

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


## patchPaymentRequestByTransactionIdRefreshStatus

> PaymentRequestRefreshStatus patchPaymentRequestByTransactionIdRefreshStatus(transactionId)

Refresh payment request status

Refresh the status of a payment request by transaction ID. Requires secret API key.

### Example

```ts
import {
  Configuration,
  PaymentRequestApi,
} from '@moosyl/sdk';
import type { PatchPaymentRequestByTransactionIdRefreshStatusRequest } from '@moosyl/sdk';

async function example() {
  console.log("🚀 Testing @moosyl/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKey
    apiKey: "YOUR API KEY",
  });
  const api = new PaymentRequestApi(config);

  const body = {
    // string
    transactionId: transactionId_example,
  } satisfies PatchPaymentRequestByTransactionIdRefreshStatusRequest;

  try {
    const data = await api.patchPaymentRequestByTransactionIdRefreshStatus(body);
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
| **transactionId** | `string` |  | [Defaults to `undefined`] |

### Return type

[**PaymentRequestRefreshStatus**](PaymentRequestRefreshStatus.md)

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


## postPaymentRequest

> PaymentRequestGet postPaymentRequest(paymentRequestCreate)

Create payment request

Create a new payment request that can be used to collect payments. Requires secret API key.

### Example

```ts
import {
  Configuration,
  PaymentRequestApi,
} from '@moosyl/sdk';
import type { PostPaymentRequestRequest } from '@moosyl/sdk';

async function example() {
  console.log("🚀 Testing @moosyl/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKey
    apiKey: "YOUR API KEY",
  });
  const api = new PaymentRequestApi(config);

  const body = {
    // PaymentRequestCreate
    paymentRequestCreate: ...,
  } satisfies PostPaymentRequestRequest;

  try {
    const data = await api.postPaymentRequest(body);
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
| **paymentRequestCreate** | [PaymentRequestCreate](PaymentRequestCreate.md) |  | |

### Return type

[**PaymentRequestGet**](PaymentRequestGet.md)

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

