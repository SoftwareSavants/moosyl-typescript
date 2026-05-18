
# ConfigurationListDataInner


## Properties

Name | Type
------------ | -------------
`id` | string
`type` | string
`organizationId` | string
`config` | any
`isTestingMode` | boolean

## Example

```typescript
import type { ConfigurationListDataInner } from '@moosyl/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "type": null,
  "organizationId": null,
  "config": null,
  "isTestingMode": null,
} satisfies ConfigurationListDataInner

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ConfigurationListDataInner
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


