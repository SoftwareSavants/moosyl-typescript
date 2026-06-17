
# PaymentGetData


## Properties

Name | Type
------------ | -------------
`id` | string
`amount` | number
`phoneNumber` | string
`passCode` | string
`status` | string
`environmentId` | string
`paymentRequestId` | string
`configurationId` | string
`referenceId` | string
`metadata` | any
`payoutId` | string
`completedAt` | Date
`createdAt` | Date
`updatedAt` | Date

## Example

```typescript
import type { PaymentGetData } from '@moosyl/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "amount": null,
  "phoneNumber": null,
  "passCode": null,
  "status": null,
  "environmentId": null,
  "paymentRequestId": null,
  "configurationId": null,
  "referenceId": null,
  "metadata": null,
  "payoutId": null,
  "completedAt": null,
  "createdAt": null,
  "updatedAt": null,
} satisfies PaymentGetData

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as PaymentGetData
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


