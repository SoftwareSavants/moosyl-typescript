
# ProductGetWithPricesData


## Properties

Name | Type
------------ | -------------
`id` | string
`organizationId` | string
`environmentId` | string
`name` | string
`description` | string
`active` | boolean
`createdAt` | Date
`prices` | [Array&lt;ProductGetWithPricesDataPricesInner&gt;](ProductGetWithPricesDataPricesInner.md)

## Example

```typescript
import type { ProductGetWithPricesData } from '@moosyl/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "organizationId": null,
  "environmentId": null,
  "name": null,
  "description": null,
  "active": null,
  "createdAt": null,
  "prices": null,
} satisfies ProductGetWithPricesData

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ProductGetWithPricesData
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


