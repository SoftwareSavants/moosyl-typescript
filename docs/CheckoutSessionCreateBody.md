
# CheckoutSessionCreateBody


## Properties

Name | Type
------------ | -------------
`paymentRequestId` | string
`transactionId` | string
`amount` | [GetProductsPageParameter](GetProductsPageParameter.md)
`phoneNumber` | string
`successUrl` | string
`cancelUrl` | string
`expiresInMinutes` | number

## Example

```typescript
import type { CheckoutSessionCreateBody } from '@moosyl/sdk'

// TODO: Update the object below with actual values
const example = {
  "paymentRequestId": null,
  "transactionId": null,
  "amount": null,
  "phoneNumber": null,
  "successUrl": null,
  "cancelUrl": null,
  "expiresInMinutes": null,
} satisfies CheckoutSessionCreateBody

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as CheckoutSessionCreateBody
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


