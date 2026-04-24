# DomainApi

All URIs are relative to *https://setup.platon.sk/api*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**changeDomainNameservers**](#changedomainnameservers) | **PATCH** /domains/{domain}/nameservers | Change domain nameservers|
|[**closeDomain**](#closedomain) | **DELETE** /domains/{domain} | Close external customer domain product|
|[**getDomainInfo**](#getdomaininfo) | **GET** /domains/{domain} | Get domain information and availability|
|[**listDomains**](#listdomains) | **GET** /domains | List customer domains|
|[**registerDomain**](#registerdomain) | **POST** /domains/{domain}/register | Register domain|
|[**renewDomain**](#renewdomain) | **POST** /domains/{domain}/renew | Renew domain|

# **changeDomainNameservers**
> CreateDnsRecord200Response changeDomainNameservers(changeDomainNameserversRequest)


### Example

```typescript
import {
    DomainApi,
    Configuration,
    ChangeDomainNameserversRequest
} from 'cp-typescript-sdk';

const configuration = new Configuration();
const apiInstance = new DomainApi(configuration);

let domain: string; //Domain name (default to undefined)
let changeDomainNameserversRequest: ChangeDomainNameserversRequest; //Nameserver payload

const { status, data } = await apiInstance.changeDomainNameservers(
    domain,
    changeDomainNameserversRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **changeDomainNameserversRequest** | **ChangeDomainNameserversRequest**| Nameserver payload | |
| **domain** | [**string**] | Domain name | defaults to undefined|


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
|**200** | Domain nameserver change response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **closeDomain**
> CreateDnsRecord200Response closeDomain()


### Example

```typescript
import {
    DomainApi,
    Configuration
} from 'cp-typescript-sdk';

const configuration = new Configuration();
const apiInstance = new DomainApi(configuration);

let domain: string; //Domain name (default to undefined)
let cname: string; //Customer name (default to undefined)

const { status, data } = await apiInstance.closeDomain(
    domain,
    cname
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **domain** | [**string**] | Domain name | defaults to undefined|
| **cname** | [**string**] | Customer name | defaults to undefined|


### Return type

**CreateDnsRecord200Response**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Domain close response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getDomainInfo**
> CreateDnsRecord200Response getDomainInfo()


### Example

```typescript
import {
    DomainApi,
    Configuration
} from 'cp-typescript-sdk';

const configuration = new Configuration();
const apiInstance = new DomainApi(configuration);

let domain: string; //Domain name (default to undefined)
let cname: string; //Customer name for product context (optional) (default to undefined)

const { status, data } = await apiInstance.getDomainInfo(
    domain,
    cname
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **domain** | [**string**] | Domain name | defaults to undefined|
| **cname** | [**string**] | Customer name for product context | (optional) defaults to undefined|


### Return type

**CreateDnsRecord200Response**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Domain info response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **listDomains**
> ListDomains200Response listDomains()


### Example

```typescript
import {
    DomainApi,
    Configuration
} from 'cp-typescript-sdk';

const configuration = new Configuration();
const apiInstance = new DomainApi(configuration);

let cname: string; //Customer name (default to undefined)

const { status, data } = await apiInstance.listDomains(
    cname
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **cname** | [**string**] | Customer name | defaults to undefined|


### Return type

**ListDomains200Response**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Domain list response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **registerDomain**
> CreateDnsRecord200Response registerDomain(registerDomainRequest)


### Example

```typescript
import {
    DomainApi,
    Configuration,
    RegisterDomainRequest
} from 'cp-typescript-sdk';

const configuration = new Configuration();
const apiInstance = new DomainApi(configuration);

let domain: string; //Domain name (default to undefined)
let registerDomainRequest: RegisterDomainRequest; //Domain registration payload

const { status, data } = await apiInstance.registerDomain(
    domain,
    registerDomainRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **registerDomainRequest** | **RegisterDomainRequest**| Domain registration payload | |
| **domain** | [**string**] | Domain name | defaults to undefined|


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
|**200** | Domain register response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **renewDomain**
> CreateDnsRecord200Response renewDomain()


### Example

```typescript
import {
    DomainApi,
    Configuration,
    RenewDomainRequest
} from 'cp-typescript-sdk';

const configuration = new Configuration();
const apiInstance = new DomainApi(configuration);

let domain: string; //Domain name (default to undefined)
let renewDomainRequest: RenewDomainRequest; //Domain renewal payload (optional)

const { status, data } = await apiInstance.renewDomain(
    domain,
    renewDomainRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **renewDomainRequest** | **RenewDomainRequest**| Domain renewal payload | |
| **domain** | [**string**] | Domain name | defaults to undefined|


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
|**200** | Domain renew response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

