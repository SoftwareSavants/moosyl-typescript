
# SubscriptionList


## Properties

Name | Type
------------ | -------------
`data` | [Array&lt;SubscriptionGetData&gt;](SubscriptionGetData.md)
`pagination` | [ProductListPagination](ProductListPagination.md)

## Example

```typescript
import type { SubscriptionList } from '@moosyl/sdk'

// TODO: Update the object below with actual values
const example = {
  "data": null,
  "pagination": null,
} satisfies SubscriptionList

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as SubscriptionList
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


