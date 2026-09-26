
# PostConnectExchangeRequest


## Properties

Name | Type
------------ | -------------
`platformId` | string
`platformSecret` | string
`code` | string
`webhookPaymentCreatedEndpoint` | string
`webhookPaymentUpdatedEndpoint` | string

## Example

```typescript
import type { PostConnectExchangeRequest } from '@moosyl/sdk'

// TODO: Update the object below with actual values
const example = {
  "platformId": null,
  "platformSecret": null,
  "code": null,
  "webhookPaymentCreatedEndpoint": null,
  "webhookPaymentUpdatedEndpoint": null,
} satisfies PostConnectExchangeRequest

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as PostConnectExchangeRequest
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


