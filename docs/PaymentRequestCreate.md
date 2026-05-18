
# PaymentRequestCreate


## Properties

Name | Type
------------ | -------------
`phoneNumber` | string
`transactionId` | string
`amount` | [GetProductsPageParameter](GetProductsPageParameter.md)

## Example

```typescript
import type { PaymentRequestCreate } from '@moosyl/sdk'

// TODO: Update the object below with actual values
const example = {
  "phoneNumber": null,
  "transactionId": null,
  "amount": null,
} satisfies PaymentRequestCreate

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as PaymentRequestCreate
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


