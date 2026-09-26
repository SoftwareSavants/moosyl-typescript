
# ConfigurationCreateData


## Properties

Name | Type
------------ | -------------
`type` | string
`config` | any
`organizationId` | string
`isTestingMode` | boolean

## Example

```typescript
import type { ConfigurationCreateData } from '@moosyl/sdk'

// TODO: Update the object below with actual values
const example = {
  "type": null,
  "config": null,
  "organizationId": null,
  "isTestingMode": null,
} satisfies ConfigurationCreateData

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ConfigurationCreateData
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


