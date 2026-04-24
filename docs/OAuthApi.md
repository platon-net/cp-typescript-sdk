# OAuthApi

All URIs are relative to *https://setup.platon.sk/api*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createOauthRequest**](#createoauthrequest) | **POST** /oauth/requests | Create OAuth request|
|[**deleteOauthToken**](#deleteoauthtoken) | **DELETE** /oauth/tokens | Delete OAuth token|
|[**getOauthScopes**](#getoauthscopes) | **GET** /oauth/scopes | List available OAuth scopes|
|[**refreshOauthToken**](#refreshoauthtoken) | **POST** /oauth/tokens/refresh | Refresh OAuth token|
|[**verifyOauthRequest**](#verifyoauthrequest) | **GET** /oauth/requests/verify | Verify OAuth request|

# **createOauthRequest**
> CreateOauthRequest200Response createOauthRequest()


### Example

```typescript
import {
    OAuthApi,
    Configuration,
    CreateOauthRequestRequest
} from '@platon-net/cp-typescript-sdk';

const configuration = new Configuration();
const apiInstance = new OAuthApi(configuration);

let createOauthRequestRequest: CreateOauthRequestRequest; //OAuth create payload (optional)

const { status, data } = await apiInstance.createOauthRequest(
    createOauthRequestRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createOauthRequestRequest** | **CreateOauthRequestRequest**| OAuth create payload | |


### Return type

**CreateOauthRequest200Response**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | OAuth create response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **deleteOauthToken**
> DeleteOauthToken200Response deleteOauthToken()


### Example

```typescript
import {
    OAuthApi,
    Configuration
} from '@platon-net/cp-typescript-sdk';

const configuration = new Configuration();
const apiInstance = new OAuthApi(configuration);

let token: string; //OAuth token (default to undefined)

const { status, data } = await apiInstance.deleteOauthToken(
    token
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **token** | [**string**] | OAuth token | defaults to undefined|


### Return type

**DeleteOauthToken200Response**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | OAuth delete response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getOauthScopes**
> GetOauthScopes200Response getOauthScopes()


### Example

```typescript
import {
    OAuthApi,
    Configuration
} from '@platon-net/cp-typescript-sdk';

const configuration = new Configuration();
const apiInstance = new OAuthApi(configuration);

const { status, data } = await apiInstance.getOauthScopes();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**GetOauthScopes200Response**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | OAuth scopes response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **refreshOauthToken**
> VerifyOauthRequest200Response refreshOauthToken(refreshOauthTokenRequest)


### Example

```typescript
import {
    OAuthApi,
    Configuration,
    RefreshOauthTokenRequest
} from '@platon-net/cp-typescript-sdk';

const configuration = new Configuration();
const apiInstance = new OAuthApi(configuration);

let refreshOauthTokenRequest: RefreshOauthTokenRequest; //OAuth refresh payload

const { status, data } = await apiInstance.refreshOauthToken(
    refreshOauthTokenRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **refreshOauthTokenRequest** | **RefreshOauthTokenRequest**| OAuth refresh payload | |


### Return type

**VerifyOauthRequest200Response**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | OAuth refresh response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **verifyOauthRequest**
> VerifyOauthRequest200Response verifyOauthRequest()


### Example

```typescript
import {
    OAuthApi,
    Configuration
} from '@platon-net/cp-typescript-sdk';

const configuration = new Configuration();
const apiInstance = new OAuthApi(configuration);

let verifyToken: string; //Verify token from OAuth create response (default to undefined)

const { status, data } = await apiInstance.verifyOauthRequest(
    verifyToken
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **verifyToken** | [**string**] | Verify token from OAuth create response | defaults to undefined|


### Return type

**VerifyOauthRequest200Response**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | OAuth verify response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

