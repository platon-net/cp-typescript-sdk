# DNSApi

All URIs are relative to *https://setup.platon.sk/api*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createDnsRecord**](#creatednsrecord) | **POST** /dns/{domain}/records | Create DNS record|
|[**deleteDnsRecord**](#deletednsrecord) | **DELETE** /dns/{domain}/records/{recordId} | Delete DNS record|
|[**getDnsRecords**](#getdnsrecords) | **GET** /dns/{domain}/records | Get DNS records by domain|
|[**updateDnsRecord**](#updatednsrecord) | **PATCH** /dns/{domain}/records/{recordId} | Update DNS record|

# **createDnsRecord**
> CreateDnsRecord200Response createDnsRecord(createDnsRecordRequest)


### Example

```typescript
import {
    DNSApi,
    Configuration,
    CreateDnsRecordRequest
} from '@platon-net/cp-typescript-sdk';

const configuration = new Configuration();
const apiInstance = new DNSApi(configuration);

let domain: string; //Domain name (default to undefined)
let createDnsRecordRequest: CreateDnsRecordRequest; //DNS record payload

const { status, data } = await apiInstance.createDnsRecord(
    domain,
    createDnsRecordRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createDnsRecordRequest** | **CreateDnsRecordRequest**| DNS record payload | |
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
|**200** | DNS record create response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **deleteDnsRecord**
> CreateDnsRecord200Response deleteDnsRecord()


### Example

```typescript
import {
    DNSApi,
    Configuration
} from '@platon-net/cp-typescript-sdk';

const configuration = new Configuration();
const apiInstance = new DNSApi(configuration);

let domain: string; //Domain name (default to undefined)
let recordId: number; //Record ID (default to undefined)

const { status, data } = await apiInstance.deleteDnsRecord(
    domain,
    recordId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **domain** | [**string**] | Domain name | defaults to undefined|
| **recordId** | [**number**] | Record ID | defaults to undefined|


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
|**200** | DNS record delete response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getDnsRecords**
> GetDnsRecords200Response getDnsRecords()


### Example

```typescript
import {
    DNSApi,
    Configuration
} from '@platon-net/cp-typescript-sdk';

const configuration = new Configuration();
const apiInstance = new DNSApi(configuration);

let domain: string; //Domain name (default to undefined)
let type: string; //Filter records by type (optional) (default to undefined)

const { status, data } = await apiInstance.getDnsRecords(
    domain,
    type
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **domain** | [**string**] | Domain name | defaults to undefined|
| **type** | [**string**] | Filter records by type | (optional) defaults to undefined|


### Return type

**GetDnsRecords200Response**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | DNS records response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **updateDnsRecord**
> CreateDnsRecord200Response updateDnsRecord(updateDnsRecordRequest)


### Example

```typescript
import {
    DNSApi,
    Configuration,
    UpdateDnsRecordRequest
} from '@platon-net/cp-typescript-sdk';

const configuration = new Configuration();
const apiInstance = new DNSApi(configuration);

let domain: string; //Domain name (default to undefined)
let recordId: number; //Record ID (default to undefined)
let updateDnsRecordRequest: UpdateDnsRecordRequest; //Partial DNS record payload

const { status, data } = await apiInstance.updateDnsRecord(
    domain,
    recordId,
    updateDnsRecordRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **updateDnsRecordRequest** | **UpdateDnsRecordRequest**| Partial DNS record payload | |
| **domain** | [**string**] | Domain name | defaults to undefined|
| **recordId** | [**number**] | Record ID | defaults to undefined|


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
|**200** | DNS record update response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

