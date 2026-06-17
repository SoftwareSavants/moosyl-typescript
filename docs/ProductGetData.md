
# ProductGetData


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

## Example

```typescript
import type { ProductGetData } from '@moosyl/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "organizationId": null,
  "environmentId": null,
  "name": null,
  "description": null,
  "active": null,
  "createdAt": null,
} satisfies ProductGetData

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ProductGetData
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


