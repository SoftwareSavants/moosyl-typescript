
# CheckoutSessionCreate


## Properties

Name | Type
------------ | -------------
`data` | [CheckoutSessionCreateData](CheckoutSessionCreateData.md)
`checkoutUrl` | string

## Example

```typescript
import type { CheckoutSessionCreate } from '@moosyl/sdk'

// TODO: Update the object below with actual values
const example = {
  "data": null,
  "checkoutUrl": null,
} satisfies CheckoutSessionCreate

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as CheckoutSessionCreate
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


