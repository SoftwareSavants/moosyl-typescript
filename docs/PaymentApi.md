# PaymentApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**getPaymentById**](PaymentApi.md#getpaymentbyid) | **GET** /payment/{id} | Get payment details |
| [**postPayment**](PaymentApi.md#postpayment) | **POST** /payment | Create a new payment |



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


## postPayment

> PostPayment200Response postPayment(paymentCreate)

Create a new payment

Use this endpoint to create a new payment for an existing payment request.  **Testing (Sandbox Environment Only)**  | Phone Number | Status     | |--------------|------------| | 22222222     | Accepted   | | 33333333     | Accepted   | | 44444444     | Accepted   | | Other        | Rejected   |

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

