
# PaymentCreate


## Properties

Name | Type
------------ | -------------
`configurationId` | string
`transactionId` | string
`phoneNumber` | string
`passCode` | string

## Example

```typescript
import type { PaymentCreate } from '@moosyl/sdk'

// TODO: Update the object below with actual values
const example = {
  "configurationId": null,
  "transactionId": null,
  "phoneNumber": null,
  "passCode": null,
} satisfies PaymentCreate

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as PaymentCreate
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


