# AuthApi

All URIs are relative to *https://setup.platon.sk/api*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createAuthToken**](#createauthtoken) | **POST** /auth/token | Create anonymous auth token|

# **createAuthToken**
> CreateAuthToken200Response createAuthToken()


### Example

```typescript
import {
    AuthApi,
    Configuration
} from '@platon-net/cp-typescript-sdk';

const configuration = new Configuration();
const apiInstance = new AuthApi(configuration);

const { status, data } = await apiInstance.createAuthToken();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**CreateAuthToken200Response**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Anonymous auth token response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

