# PaymentApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**getPaymentById**](PaymentApi.md#getpaymentbyid) | **GET** /payment/{id} | Get payment details |
| [**getPaymentByIdStatus**](PaymentApi.md#getpaymentbyidstatus) | **GET** /payment/{id}/status | Get payment status (heartbeat) |
| [**postPayment**](PaymentApi.md#postpayment) | **POST** /payment | Create a new payment |
| [**postPaymentByIdSimulateTransfer**](PaymentApi.md#postpaymentbyidsimulatetransfer) | **POST** /payment/{id}/simulate-transfer | Simulate a Gimtel transfer (sandbox) |



## getPaymentById

> PaymentGet getPaymentById(id)

Get payment details

Retrieve detailed information about a payment by transaction ID. Requires secret API key.

### Example

```ts
import {
  Configuration,
  PaymentApi,
} from '@moosyl/sdk';
import type { GetPaymentByIdRequest } from '@moosyl/sdk';

async function example() {
  console.log("🚀 Testing @moosyl/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKey
    apiKey: "YOUR API KEY",
  });
  const api = new PaymentApi(config);

  const body = {
    // string
    id: id_example,
  } satisfies GetPaymentByIdRequest;

  try {
    const data = await api.getPaymentById(body);
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

[**PaymentGet**](PaymentGet.md)

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


## getPaymentByIdStatus

> GetPaymentByIdStatus200Response getPaymentByIdStatus(id)

Get payment status (heartbeat)

Returns the payment\&#39;s status. For Gimtel payments, poll this every few seconds while the payer is on the payment screen: the payment stops being claimable about 10 minutes after the last poll.

### Example

```ts
import {
  Configuration,
  PaymentApi,
} from '@moosyl/sdk';
import type { GetPaymentByIdStatusRequest } from '@moosyl/sdk';

async function example() {
  console.log("🚀 Testing @moosyl/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKey
    apiKey: "YOUR API KEY",
  });
  const api = new PaymentApi(config);

  const body = {
    // string
    id: id_example,
  } satisfies GetPaymentByIdStatusRequest;

  try {
    const data = await api.getPaymentByIdStatus(body);
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

[**GetPaymentByIdStatus200Response**](GetPaymentByIdStatus200Response.md)

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


## postPayment

> PostPayment200Response postPayment(paymentCreate)

Create a new payment

Use this endpoint to create a new payment for an existing payment request.  **Testing (Sandbox Environment Only) — native methods only**  The magic phone numbers below only apply to native payment methods (e.g. Sedad, NexConnect, native Bankily). They do not apply to Gimtel methods — see below.  | Phone Number | Status     | |--------------|------------| | 22222222     | Accepted   | | 33333333     | Accepted   | | 44444444     | Accepted   | | Other        | Rejected   |  **Gimtel methods (Bankily via Gimtel, BCI Pay, Amanty)**  The payment is created as &#x60;pending&#x60; and the response includes &#x60;instructions&#x60; (receiving phone, exact amount). The payer transfers from the phone number you sent. Poll &#x60;GET /payment/{paymentId}/status&#x60; every few seconds while the payer is on the payment screen — the payment stops being claimable about 10 minutes after the last poll. Completion also fires the &#x60;payment-updated&#x60; webhook.  In sandbox, Gimtel methods are never completed by a magic phone number: call &#x60;POST /payment/{paymentId}/simulate-transfer&#x60; instead to simulate the payer\&#39;s bank transfer and complete the payment.

### Example

```ts
import {
  Configuration,
  PaymentApi,
} from '@moosyl/sdk';
import type { PostPaymentRequest } from '@moosyl/sdk';

async function example() {
  console.log("🚀 Testing @moosyl/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKey
    apiKey: "YOUR API KEY",
  });
  const api = new PaymentApi(config);

  const body = {
    // PaymentCreate
    paymentCreate: ...,
  } satisfies PostPaymentRequest;

  try {
    const data = await api.postPayment(body);
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
| **paymentCreate** | [PaymentCreate](PaymentCreate.md) |  | |

### Return type

[**PostPayment200Response**](PostPayment200Response.md)

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


## postPaymentByIdSimulateTransfer

> PostPaymentByIdSimulateTransfer200Response postPaymentByIdSimulateTransfer(id)

Simulate a Gimtel transfer (sandbox)

Sandbox only. Completes a pending Gimtel payment as if the payer had transferred the exact amount.

### Example

```ts
import {
  Configuration,
  PaymentApi,
} from '@moosyl/sdk';
import type { PostPaymentByIdSimulateTransferRequest } from '@moosyl/sdk';

async function example() {
  console.log("🚀 Testing @moosyl/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKey
    apiKey: "YOUR API KEY",
  });
  const api = new PaymentApi(config);

  const body = {
    // string
    id: id_example,
  } satisfies PostPaymentByIdSimulateTransferRequest;

  try {
    const data = await api.postPaymentByIdSimulateTransfer(body);
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

[**PostPaymentByIdSimulateTransfer200Response**](PostPaymentByIdSimulateTransfer200Response.md)

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

