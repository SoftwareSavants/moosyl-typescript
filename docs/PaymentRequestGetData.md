
# PaymentRequestGetData


## Properties

Name | Type
------------ | -------------
`id` | string
`amount` | number
`totalAmount` | number
`phoneNumber` | string
`transactionId` | string
`environmentId` | string
`retryCount` | number
`createdAt` | Date
`updatedAt` | Date

## Example

```typescript
import type { PaymentRequestGetData } from '@moosyl/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "amount": null,
  "totalAmount": null,
  "phoneNumber": null,
  "transactionId": null,
  "environmentId": null,
  "retryCount": null,
  "createdAt": null,
  "updatedAt": null,
} satisfies PaymentRequestGetData

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as PaymentRequestGetData
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


