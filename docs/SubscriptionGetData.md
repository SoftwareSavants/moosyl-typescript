
# SubscriptionGetData


## Properties

Name | Type
------------ | -------------
`id` | string
`organizationId` | string
`customerId` | string
`priceId` | string
`status` | string
`nextBillingDate` | Date
`startedAt` | Date
`cancelledAt` | Date
`expiresAt` | Date

## Example

```typescript
import type { SubscriptionGetData } from '@moosyl/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "organizationId": null,
  "customerId": null,
  "priceId": null,
  "status": null,
  "nextBillingDate": null,
  "startedAt": null,
  "cancelledAt": null,
  "expiresAt": null,
} satisfies SubscriptionGetData

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as SubscriptionGetData
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


