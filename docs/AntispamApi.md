# AntispamApi

All URIs are relative to *https://setup.platon.sk/api*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**addAntispamMaildata**](#addantispammaildata) | **POST** /antispam/maildata | Add maildata to antispam engine|
|[**checkAntispamMaildataRules**](#checkantispammaildatarules) | **POST** /antispam/maildata/check | Check maildata against existing antispam rules|
|[**createAntispamEmailRule**](#createantispamemailrule) | **POST** /antispam/rules | Create antispam email rule or increment existing rule hitcount|

# **addAntispamMaildata**
> CreateDnsRecord200Response addAntispamMaildata(addAntispamMaildataRequest)


### Example

```typescript
import {
    AntispamApi,
    Configuration,
    AddAntispamMaildataRequest
} from '@platon-net/cp-typescript-sdk';

const configuration = new Configuration();
const apiInstance = new AntispamApi(configuration);

let addAntispamMaildataRequest: AddAntispamMaildataRequest; //Maildata payload

const { status, data } = await apiInstance.addAntispamMaildata(
    addAntispamMaildataRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **addAntispamMaildataRequest** | **AddAntispamMaildataRequest**| Maildata payload | |


### Return type

**CreateDnsRecord200Response**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Antispam maildata add response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **checkAntispamMaildataRules**
> CreateDnsRecord200Response checkAntispamMaildataRules(checkAntispamMaildataRulesRequest)


### Example

```typescript
import {
    AntispamApi,
    Configuration,
    CheckAntispamMaildataRulesRequest
} from '@platon-net/cp-typescript-sdk';

const configuration = new Configuration();
const apiInstance = new AntispamApi(configuration);

let checkAntispamMaildataRulesRequest: CheckAntispamMaildataRulesRequest; //Maildata payload

const { status, data } = await apiInstance.checkAntispamMaildataRules(
    checkAntispamMaildataRulesRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **checkAntispamMaildataRulesRequest** | **CheckAntispamMaildataRulesRequest**| Maildata payload | |


### Return type

**CreateDnsRecord200Response**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Maildata antispam check response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **createAntispamEmailRule**
> CreateDnsRecord200Response createAntispamEmailRule(createAntispamEmailRuleRequest)


### Example

```typescript
import {
    AntispamApi,
    Configuration,
    CreateAntispamEmailRuleRequest
} from '@platon-net/cp-typescript-sdk';

const configuration = new Configuration();
const apiInstance = new AntispamApi(configuration);

let createAntispamEmailRuleRequest: CreateAntispamEmailRuleRequest; //Antispam email rule payload

const { status, data } = await apiInstance.createAntispamEmailRule(
    createAntispamEmailRuleRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createAntispamEmailRuleRequest** | **CreateAntispamEmailRuleRequest**| Antispam email rule payload | |


### Return type

**CreateDnsRecord200Response**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Antispam rule create response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

