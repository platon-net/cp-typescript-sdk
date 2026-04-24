# EmailApi

All URIs are relative to *https://setup.platon.sk/api*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**changeMailboxPassword**](#changemailboxpassword) | **PATCH** /email/{domain}/mailboxes/{username}/password | Change mailbox password|
|[**createMailbox**](#createmailbox) | **POST** /email/{domain}/mailboxes | Create mailbox|

# **changeMailboxPassword**
> CreateDnsRecord200Response changeMailboxPassword(changeMailboxPasswordRequest)


### Example

```typescript
import {
    EmailApi,
    Configuration,
    ChangeMailboxPasswordRequest
} from 'cp-typescript-sdk';

const configuration = new Configuration();
const apiInstance = new EmailApi(configuration);

let domain: string; //Domain name (default to undefined)
let username: string; //Mailbox username (default to undefined)
let changeMailboxPasswordRequest: ChangeMailboxPasswordRequest; //Mailbox password payload

const { status, data } = await apiInstance.changeMailboxPassword(
    domain,
    username,
    changeMailboxPasswordRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **changeMailboxPasswordRequest** | **ChangeMailboxPasswordRequest**| Mailbox password payload | |
| **domain** | [**string**] | Domain name | defaults to undefined|
| **username** | [**string**] | Mailbox username | defaults to undefined|


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
|**200** | Mailbox password change response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **createMailbox**
> CreateDnsRecord200Response createMailbox(createMailboxRequest)


### Example

```typescript
import {
    EmailApi,
    Configuration,
    CreateMailboxRequest
} from 'cp-typescript-sdk';

const configuration = new Configuration();
const apiInstance = new EmailApi(configuration);

let domain: string; //Domain name (default to undefined)
let createMailboxRequest: CreateMailboxRequest; //Mailbox payload

const { status, data } = await apiInstance.createMailbox(
    domain,
    createMailboxRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createMailboxRequest** | **CreateMailboxRequest**| Mailbox payload | |
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
|**200** | Mailbox create response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

