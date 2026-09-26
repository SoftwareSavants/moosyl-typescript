# InvoicesApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**getInvoices**](InvoicesApi.md#getinvoices) | **GET** /invoices/ | List invoices or filter by id/external user |



## getInvoices

> InvoiceList getInvoices(id, externalUserId, subscriptionId, page, limit)

List invoices or filter by id/external user

### Example

```ts
import {
  Configuration,
  InvoicesApi,
} from '@moosyl/sdk';
import type { GetInvoicesRequest } from '@moosyl/sdk';

async function example() {
  console.log("🚀 Testing @moosyl/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKey
    apiKey: "YOUR API KEY",
  });
  const api = new InvoicesApi(config);

  const body = {
    // string (optional)
    id: id_example,
    // string (optional)
    externalUserId: externalUserId_example,
    // string (optional)
    subscriptionId: subscriptionId_example,
    // GetProductsPageParameter (optional)
    page: ...,
    // GetProductsPageParameter (optional)
    limit: ...,
  } satisfies GetInvoicesRequest;

  try {
    const data = await api.getInvoices(body);
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
| **subscriptionId** | `string` |  | [Optional] [Defaults to `undefined`] |
| **page** | [](.md) |  | [Optional] [Defaults to `undefined`] |
| **limit** | [](.md) |  | [Optional] [Defaults to `undefined`] |

### Return type

[**InvoiceList**](InvoiceList.md)

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

