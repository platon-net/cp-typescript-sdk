# SpamDetection200ResponseData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**classification** | **string** | Normalized classification returned by the LLM. | [default to undefined]
**confidence** | **number** | Normalized confidence from 0 to 100. | [default to undefined]
**reason** | **string** | Short explanation in Slovak. | [default to undefined]
**signals** | **Array&lt;string&gt;** | Most important signals used for the classification. | [default to undefined]
**error** | **boolean** | True when the LLM call or response validation failed. | [default to undefined]
**error_message** | **string** | Short technical error reason. Raw LLM response is never returned here. | [default to undefined]

## Example

```typescript
import { SpamDetection200ResponseData } from '@platon-net/cp-typescript-sdk';

const instance: SpamDetection200ResponseData = {
    classification,
    confidence,
    reason,
    signals,
    error,
    error_message,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
