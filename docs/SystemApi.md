# SystemApi

All URIs are relative to *https://setup.platon.sk/api*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**hello**](#hello) | **GET** /system/hello | Returns greeting message|
|[**revision**](#revision) | **GET** /system/revision | Returns revision number of system|
|[**time**](#time) | **GET** /system/time | Returns current date and time of system|

# **hello**
> Hello200Response hello()


### Example

```typescript
import {
    SystemApi,
    Configuration
} from '@platon-net/cp-typescript-sdk';

const configuration = new Configuration();
const apiInstance = new SystemApi(configuration);

const { status, data } = await apiInstance.hello();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**Hello200Response**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **revision**
> Revision200Response revision()


### Example

```typescript
import {
    SystemApi,
    Configuration
} from '@platon-net/cp-typescript-sdk';

const configuration = new Configuration();
const apiInstance = new SystemApi(configuration);

const { status, data } = await apiInstance.revision();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**Revision200Response**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **time**
> Time200Response time()


### Example

```typescript
import {
    SystemApi,
    Configuration
} from '@platon-net/cp-typescript-sdk';

const configuration = new Configuration();
const apiInstance = new SystemApi(configuration);

const { status, data } = await apiInstance.time();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**Time200Response**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

