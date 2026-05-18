
# PriceUpdate


## Properties

Name | Type
------------ | -------------
`amount` | [PriceUpdateAmount](PriceUpdateAmount.md)
`interval` | string
`replaceExisting` | boolean

## Example

```typescript
import type { PriceUpdate } from '@moosyl/sdk'

// TODO: Update the object below with actual values
const example = {
  "amount": null,
  "interval": null,
  "replaceExisting": null,
} satisfies PriceUpdate

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as PriceUpdate
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


