
# SubscriptionCreate


## Properties

Name | Type
------------ | -------------
`id` | string
`customerId` | string
`priceId` | string
`cancelledAt` | Date
`expiresAt` | Date
`trial` | [SubscriptionCreateTrial](SubscriptionCreateTrial.md)
`trialPeriod` | string
`trialEnd` | [SubscriptionCreateTrialEnd](SubscriptionCreateTrialEnd.md)
`startedAt` | [SubscriptionCreateTrialEnd](SubscriptionCreateTrialEnd.md)

## Example

```typescript
import type { SubscriptionCreate } from '@moosyl/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "customerId": null,
  "priceId": null,
  "cancelledAt": null,
  "expiresAt": null,
  "trial": null,
  "trialPeriod": null,
  "trialEnd": null,
  "startedAt": null,
} satisfies SubscriptionCreate

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as SubscriptionCreate
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


