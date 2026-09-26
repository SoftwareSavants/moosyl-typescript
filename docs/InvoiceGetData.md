
# InvoiceGetData


## Properties

Name | Type
------------ | -------------
`id` | string
`customerId` | string
`organizationId` | string
`status` | string
`amount` | string
`dueDate` | Date
`paymentRequestId` | string
`createdAt` | Date

## Example

```typescript
import type { InvoiceGetData } from '@moosyl/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "customerId": null,
  "organizationId": null,
  "status": null,
  "amount": null,
  "dueDate": null,
  "paymentRequestId": null,
  "createdAt": null,
} satisfies InvoiceGetData

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as InvoiceGetData
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


