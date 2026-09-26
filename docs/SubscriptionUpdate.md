
# SubscriptionUpdate


## Properties

Name | Type
------------ | -------------
`priceId` | string
`status` | string
`nextBillingDate` | Date
`cancelledAt` | Date
`expiresAt` | Date

## Example

```typescript
import type { SubscriptionUpdate } from '@moosyl/sdk'

// TODO: Update the object below with actual values
const example = {
  "priceId": null,
  "status": null,
  "nextBillingDate": null,
  "cancelledAt": null,
  "expiresAt": null,
} satisfies SubscriptionUpdate

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as SubscriptionUpdate
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


