
# PaymentRequestRefreshStatus


## Properties

Name | Type
------------ | -------------
`data` | [PaymentRequestGetData](PaymentRequestGetData.md)
`bankingApiResponses` | [Array&lt;PaymentRequestRefreshStatusBankingApiResponsesInner&gt;](PaymentRequestRefreshStatusBankingApiResponsesInner.md)

## Example

```typescript
import type { PaymentRequestRefreshStatus } from '@moosyl/sdk'

// TODO: Update the object below with actual values
const example = {
  "data": null,
  "bankingApiResponses": null,
} satisfies PaymentRequestRefreshStatus

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as PaymentRequestRefreshStatus
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


