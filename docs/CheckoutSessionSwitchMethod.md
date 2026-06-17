
# CheckoutSessionSwitchMethod


## Properties

Name | Type
------------ | -------------
`data` | [CheckoutSessionCreateData](CheckoutSessionCreateData.md)
`organization` | [GetOrganizationById200ResponseData](GetOrganizationById200ResponseData.md)
`paymentRequest` | [PaymentRequestGetData](PaymentRequestGetData.md)
`configurations` | [Array&lt;ConfigurationListDataInner&gt;](ConfigurationListDataInner.md)
`latestPayment` | [CheckoutSessionGetLatestPayment](CheckoutSessionGetLatestPayment.md)

## Example

```typescript
import type { CheckoutSessionSwitchMethod } from '@moosyl/sdk'

// TODO: Update the object below with actual values
const example = {
  "data": null,
  "organization": null,
  "paymentRequest": null,
  "configurations": null,
  "latestPayment": null,
} satisfies CheckoutSessionSwitchMethod

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as CheckoutSessionSwitchMethod
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


