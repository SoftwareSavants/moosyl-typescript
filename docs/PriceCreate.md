
# PriceCreate


## Properties

Name | Type
------------ | -------------
`id` | string
`productId` | string
`amount` | number
`interval` | string
`active` | boolean
`createdAt` | Date

## Example

```typescript
import type { PriceCreate } from '@moosyl/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "productId": null,
  "amount": null,
  "interval": null,
  "active": null,
  "createdAt": null,
} satisfies PriceCreate

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as PriceCreate
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


