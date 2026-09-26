
# CronResult


## Properties

Name | Type
------------ | -------------
`cancelled` | number
`expired` | number
`updated` | number
`processed` | number
`failed` | number
`total` | number
`processedAt` | string

## Example

```typescript
import type { CronResult } from '@moosyl/sdk'

// TODO: Update the object below with actual values
const example = {
  "cancelled": null,
  "expired": null,
  "updated": null,
  "processed": null,
  "failed": null,
  "total": null,
  "processedAt": null,
} satisfies CronResult

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as CronResult
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


