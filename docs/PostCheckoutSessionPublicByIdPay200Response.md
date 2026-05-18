
# PostCheckoutSessionPublicByIdPay200Response


## Properties

Name | Type
------------ | -------------
`status` | string
`referenceId` | string
`paymentCode` | string
`successUrl` | string
`provider` | string
`formData` | any

## Example

```typescript
import type { PostCheckoutSessionPublicByIdPay200Response } from '@moosyl/sdk'

// TODO: Update the object below with actual values
const example = {
  "status": null,
  "referenceId": null,
  "paymentCode": null,
  "successUrl": null,
  "provider": null,
  "formData": null,
} satisfies PostCheckoutSessionPublicByIdPay200Response

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as PostCheckoutSessionPublicByIdPay200Response
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


