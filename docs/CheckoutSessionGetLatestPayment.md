
# CheckoutSessionGetLatestPayment


## Properties

Name | Type
------------ | -------------
`id` | string
`amount` | number
`status` | string
`referenceId` | string
`paymentCode` | string

## Example

```typescript
import type { CheckoutSessionGetLatestPayment } from '@moosyl/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "amount": null,
  "status": null,
  "referenceId": null,
  "paymentCode": null,
} satisfies CheckoutSessionGetLatestPayment

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as CheckoutSessionGetLatestPayment
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


