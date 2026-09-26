
# SubscriptionCreateByExternalUser


## Properties

Name | Type
------------ | -------------
`externalUserId` | string
`phone` | string
`priceId` | string
`trial` | [SubscriptionCreateTrial](SubscriptionCreateTrial.md)
`trialPeriod` | string
`trialEnd` | [SubscriptionCreateTrialEnd](SubscriptionCreateTrialEnd.md)
`startedAt` | [SubscriptionCreateTrialEnd](SubscriptionCreateTrialEnd.md)
`expiresAt` | [SubscriptionCreateTrialEnd](SubscriptionCreateTrialEnd.md)

## Example

```typescript
import type { SubscriptionCreateByExternalUser } from '@moosyl/sdk'

// TODO: Update the object below with actual values
const example = {
  "externalUserId": null,
  "phone": null,
  "priceId": null,
  "trial": null,
  "trialPeriod": null,
  "trialEnd": null,
  "startedAt": null,
  "expiresAt": null,
} satisfies SubscriptionCreateByExternalUser

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as SubscriptionCreateByExternalUser
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


