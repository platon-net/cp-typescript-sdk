# LLMApi

All URIs are relative to *https://setup.platon.sk/api*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**spamDetection**](#spamdetection) | **POST** /llm/spam-detection | Classify a web form message as spam or ham using the local LLM|

# **spamDetection**
> SpamDetection200Response spamDetection(spamDetectionRequest)


### Example

```typescript
import {
    LLMApi,
    Configuration,
    SpamDetectionRequest
} from '@platon-net/cp-typescript-sdk';

const configuration = new Configuration();
const apiInstance = new LLMApi(configuration);

let spamDetectionRequest: SpamDetectionRequest; //Spam detection payload

const { status, data } = await apiInstance.spamDetection(
    spamDetectionRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **spamDetectionRequest** | **SpamDetectionRequest**| Spam detection payload | |


### Return type

**SpamDetection200Response**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Spam detection response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

