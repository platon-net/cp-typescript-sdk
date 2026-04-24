# VehicleApi

All URIs are relative to *https://setup.platon.sk/api*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createVehicleEvent**](#createvehicleevent) | **POST** /vehicle/events | Create vehicle event without receipt image|
|[**deleteVehicleEvent**](#deletevehicleevent) | **DELETE** /vehicle/events/{eventId} | Delete vehicle event|
|[**finalizeVehicleEvent**](#finalizevehicleevent) | **POST** /vehicle/events/{eventId}/finalize | Finalize vehicle event draft|
|[**getVehicleEvent**](#getvehicleevent) | **GET** /vehicle/events/{eventId} | Get vehicle event detail|
|[**getVehicleEventImage**](#getvehicleeventimage) | **GET** /vehicle/events/{eventId}/image | Get event image or thumbnail|
|[**listVehicleCurrencies**](#listvehiclecurrencies) | **GET** /vehicle/currencies | List currencies for vehicle events|
|[**listVehicleEvents**](#listvehicleevents) | **GET** /vehicle/events | List vehicle events for the authenticated driver|
|[**listVehicleVehicles**](#listvehiclevehicles) | **GET** /vehicle/vehicles | List vehicles available to the authenticated driver|
|[**rescanVehicleEventImage**](#rescanvehicleeventimage) | **POST** /vehicle/events/{eventId}/image | Replace event image and rescan event data|
|[**setPreferredVehicle**](#setpreferredvehicle) | **PATCH** /vehicle/preferred-vehicle | Set or clear preferred vehicle|
|[**uploadVehicleReceiptImage**](#uploadvehiclereceiptimage) | **POST** /vehicle/events/receipt-image | Upload receipt image and create processing event draft|

# **createVehicleEvent**
> CreateDnsRecord200Response createVehicleEvent(createVehicleEventRequest)


### Example

```typescript
import {
    VehicleApi,
    Configuration,
    CreateVehicleEventRequest
} from 'cp-typescript-sdk';

const configuration = new Configuration();
const apiInstance = new VehicleApi(configuration);

let createVehicleEventRequest: CreateVehicleEventRequest; //Vehicle event create payload

const { status, data } = await apiInstance.createVehicleEvent(
    createVehicleEventRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createVehicleEventRequest** | **CreateVehicleEventRequest**| Vehicle event create payload | |


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
|**200** | Vehicle event create response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **deleteVehicleEvent**
> CreateDnsRecord200Response deleteVehicleEvent()


### Example

```typescript
import {
    VehicleApi,
    Configuration
} from 'cp-typescript-sdk';

const configuration = new Configuration();
const apiInstance = new VehicleApi(configuration);

let eventId: number; //Vehicle event ID (default to undefined)

const { status, data } = await apiInstance.deleteVehicleEvent(
    eventId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **eventId** | [**number**] | Vehicle event ID | defaults to undefined|


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
|**200** | Vehicle event delete response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **finalizeVehicleEvent**
> CreateDnsRecord200Response finalizeVehicleEvent(finalizeVehicleEventRequest)


### Example

```typescript
import {
    VehicleApi,
    Configuration,
    FinalizeVehicleEventRequest
} from 'cp-typescript-sdk';

const configuration = new Configuration();
const apiInstance = new VehicleApi(configuration);

let eventId: number; //Vehicle event ID (default to undefined)
let finalizeVehicleEventRequest: FinalizeVehicleEventRequest; //Vehicle event finalize payload

const { status, data } = await apiInstance.finalizeVehicleEvent(
    eventId,
    finalizeVehicleEventRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **finalizeVehicleEventRequest** | **FinalizeVehicleEventRequest**| Vehicle event finalize payload | |
| **eventId** | [**number**] | Vehicle event ID | defaults to undefined|


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
|**200** | Vehicle event finalize response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getVehicleEvent**
> CreateDnsRecord200Response getVehicleEvent()


### Example

```typescript
import {
    VehicleApi,
    Configuration
} from 'cp-typescript-sdk';

const configuration = new Configuration();
const apiInstance = new VehicleApi(configuration);

let eventId: number; //Vehicle event ID (default to undefined)

const { status, data } = await apiInstance.getVehicleEvent(
    eventId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **eventId** | [**number**] | Vehicle event ID | defaults to undefined|


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
|**200** | Vehicle event detail response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getVehicleEventImage**
> File getVehicleEventImage()


### Example

```typescript
import {
    VehicleApi,
    Configuration
} from 'cp-typescript-sdk';

const configuration = new Configuration();
const apiInstance = new VehicleApi(configuration);

let eventId: number; //Vehicle event ID (default to undefined)
let size: string; //Image size variant: thumb, thumbnail or small for thumbnail response (optional) (default to undefined)

const { status, data } = await apiInstance.getVehicleEventImage(
    eventId,
    size
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **eventId** | [**number**] | Vehicle event ID | defaults to undefined|
| **size** | [**string**] | Image size variant: thumb, thumbnail or small for thumbnail response | (optional) defaults to undefined|


### Return type

**File**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: image/*


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Vehicle event image response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **listVehicleCurrencies**
> CreateDnsRecord200Response listVehicleCurrencies()


### Example

```typescript
import {
    VehicleApi,
    Configuration
} from 'cp-typescript-sdk';

const configuration = new Configuration();
const apiInstance = new VehicleApi(configuration);

const { status, data } = await apiInstance.listVehicleCurrencies();
```

### Parameters
This endpoint does not have any parameters.


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
|**200** | Vehicle currency list response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **listVehicleEvents**
> CreateDnsRecord200Response listVehicleEvents()


### Example

```typescript
import {
    VehicleApi,
    Configuration
} from 'cp-typescript-sdk';

const configuration = new Configuration();
const apiInstance = new VehicleApi(configuration);

let since: string; //Return events with event datetime greater than or equal to the provided local datetime (optional) (default to undefined)

const { status, data } = await apiInstance.listVehicleEvents(
    since
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **since** | [**string**] | Return events with event datetime greater than or equal to the provided local datetime | (optional) defaults to undefined|


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
|**200** | Vehicle event list response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **listVehicleVehicles**
> CreateDnsRecord200Response listVehicleVehicles()


### Example

```typescript
import {
    VehicleApi,
    Configuration
} from 'cp-typescript-sdk';

const configuration = new Configuration();
const apiInstance = new VehicleApi(configuration);

const { status, data } = await apiInstance.listVehicleVehicles();
```

### Parameters
This endpoint does not have any parameters.


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
|**200** | Vehicle list response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **rescanVehicleEventImage**
> CreateDnsRecord200Response rescanVehicleEventImage()


### Example

```typescript
import {
    VehicleApi,
    Configuration
} from 'cp-typescript-sdk';

const configuration = new Configuration();
const apiInstance = new VehicleApi(configuration);

let eventId: number; //Vehicle event ID (default to undefined)
let image: File; // (default to undefined)
let timezone: string; // (optional) (default to undefined)
let eventType: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.rescanVehicleEventImage(
    eventId,
    image,
    timezone,
    eventType
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **eventId** | [**number**] | Vehicle event ID | defaults to undefined|
| **image** | [**File**] |  | defaults to undefined|
| **timezone** | [**string**] |  | (optional) defaults to undefined|
| **eventType** | [**string**] |  | (optional) defaults to undefined|


### Return type

**CreateDnsRecord200Response**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: multipart/form-data
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Vehicle event image rescan response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **setPreferredVehicle**
> CreateDnsRecord200Response setPreferredVehicle()


### Example

```typescript
import {
    VehicleApi,
    Configuration,
    SetPreferredVehicleRequest
} from 'cp-typescript-sdk';

const configuration = new Configuration();
const apiInstance = new VehicleApi(configuration);

let setPreferredVehicleRequest: SetPreferredVehicleRequest; //Preferred vehicle payload (optional)

const { status, data } = await apiInstance.setPreferredVehicle(
    setPreferredVehicleRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **setPreferredVehicleRequest** | **SetPreferredVehicleRequest**| Preferred vehicle payload | |


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
|**200** | Preferred vehicle response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **uploadVehicleReceiptImage**
> CreateDnsRecord200Response uploadVehicleReceiptImage()


### Example

```typescript
import {
    VehicleApi,
    Configuration
} from 'cp-typescript-sdk';

const configuration = new Configuration();
const apiInstance = new VehicleApi(configuration);

let image: File; // (default to undefined)
let timezone: string; // (default to undefined)
let eventType: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.uploadVehicleReceiptImage(
    image,
    timezone,
    eventType
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **image** | [**File**] |  | defaults to undefined|
| **timezone** | [**string**] |  | defaults to undefined|
| **eventType** | [**string**] |  | (optional) defaults to undefined|


### Return type

**CreateDnsRecord200Response**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: multipart/form-data
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Vehicle receipt upload response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

