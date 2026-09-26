
# CheckoutSessionCreateData


## Properties

Name | Type
------------ | -------------
`id` | string
`paymentRequestId` | string
`environmentId` | string
`selectedConfigurationId` | string
`status` | string
`successUrl` | string
`cancelUrl` | string
`expiresAt` | Date
`completedAt` | Date
`createdAt` | Date
`updatedAt` | Date

## Example

```typescript
import type { CheckoutSessionCreateData } from '@moosyl/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "paymentRequestId": null,
  "environmentId": null,
  "selectedConfigurationId": null,
  "status": null,
  "successUrl": null,
  "cancelUrl": null,
  "expiresAt": null,
  "completedAt": null,
  "createdAt": null,
  "updatedAt": null,
} satisfies CheckoutSessionCreateData

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as CheckoutSessionCreateData
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


