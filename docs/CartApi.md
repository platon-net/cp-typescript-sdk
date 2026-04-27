# CartApi

All URIs are relative to *https://setup.platon.sk/api*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**checkCartCoupon**](#checkcartcoupon) | **POST** /cart/coupons/check | Check and apply cart coupon|
|[**createCartItem**](#createcartitem) | **POST** /cart/items | Add item to cart|
|[**deleteCartItem**](#deletecartitem) | **DELETE** /cart/items/{cartItemId} | Remove item from cart|
|[**getCartBillingAddress**](#getcartbillingaddress) | **GET** /cart/billing-address | Get cart billing address|
|[**getCartCoupon**](#getcartcoupon) | **GET** /cart/coupons/current | Get current cart coupon|
|[**getCartTotal**](#getcarttotal) | **GET** /cart/total | Get cart total|
|[**listCartItems**](#listcartitems) | **GET** /cart/items | List cart items|
|[**updateCartItem**](#updatecartitem) | **PATCH** /cart/items/{cartItemId} | Update cart item data|
|[**updateCartItemCount**](#updatecartitemcount) | **PATCH** /cart/items/by-product/count | Update cart item count by product and domain|

# **checkCartCoupon**
> CreateDnsRecord200Response checkCartCoupon(checkCartCouponRequest)


### Example

```typescript
import {
    CartApi,
    Configuration,
    CheckCartCouponRequest
} from '@platon-net/cp-typescript-sdk';

const configuration = new Configuration();
const apiInstance = new CartApi(configuration);

let checkCartCouponRequest: CheckCartCouponRequest; //Cart coupon check payload

const { status, data } = await apiInstance.checkCartCoupon(
    checkCartCouponRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **checkCartCouponRequest** | **CheckCartCouponRequest**| Cart coupon check payload | |


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
|**200** | Cart coupon check response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **createCartItem**
> CreateDnsRecord200Response createCartItem(createCartItemRequest)


### Example

```typescript
import {
    CartApi,
    Configuration,
    CreateCartItemRequest
} from '@platon-net/cp-typescript-sdk';

const configuration = new Configuration();
const apiInstance = new CartApi(configuration);

let createCartItemRequest: CreateCartItemRequest; //Cart item add payload

const { status, data } = await apiInstance.createCartItem(
    createCartItemRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createCartItemRequest** | **CreateCartItemRequest**| Cart item add payload | |


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
|**200** | Cart item add response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **deleteCartItem**
> CreateDnsRecord200Response deleteCartItem()


### Example

```typescript
import {
    CartApi,
    Configuration
} from '@platon-net/cp-typescript-sdk';

const configuration = new Configuration();
const apiInstance = new CartApi(configuration);

let cartItemId: number; //Cart item ID (default to undefined)
let cname: string; //Customer name (optional) (default to undefined)

const { status, data } = await apiInstance.deleteCartItem(
    cartItemId,
    cname
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **cartItemId** | [**number**] | Cart item ID | defaults to undefined|
| **cname** | [**string**] | Customer name | (optional) defaults to undefined|


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
|**200** | Cart item remove response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getCartBillingAddress**
> CreateDnsRecord200Response getCartBillingAddress()


### Example

```typescript
import {
    CartApi,
    Configuration
} from '@platon-net/cp-typescript-sdk';

const configuration = new Configuration();
const apiInstance = new CartApi(configuration);

let cname: string; //Customer name (optional) (default to undefined)

const { status, data } = await apiInstance.getCartBillingAddress(
    cname
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **cname** | [**string**] | Customer name | (optional) defaults to undefined|


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
|**200** | Cart billing address response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getCartCoupon**
> CreateDnsRecord200Response getCartCoupon()


### Example

```typescript
import {
    CartApi,
    Configuration
} from '@platon-net/cp-typescript-sdk';

const configuration = new Configuration();
const apiInstance = new CartApi(configuration);

let cname: string; //Customer name (optional) (default to undefined)

const { status, data } = await apiInstance.getCartCoupon(
    cname
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **cname** | [**string**] | Customer name | (optional) defaults to undefined|


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
|**200** | Current cart coupon response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getCartTotal**
> CreateDnsRecord200Response getCartTotal()


### Example

```typescript
import {
    CartApi,
    Configuration
} from '@platon-net/cp-typescript-sdk';

const configuration = new Configuration();
const apiInstance = new CartApi(configuration);

let cname: string; //Customer name (optional) (default to undefined)

const { status, data } = await apiInstance.getCartTotal(
    cname
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **cname** | [**string**] | Customer name | (optional) defaults to undefined|


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
|**200** | Cart total response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **listCartItems**
> CreateDnsRecord200Response listCartItems()


### Example

```typescript
import {
    CartApi,
    Configuration
} from '@platon-net/cp-typescript-sdk';

const configuration = new Configuration();
const apiInstance = new CartApi(configuration);

let cname: string; //Customer name (optional) (default to undefined)
let lang: string; //Response language (optional) (default to undefined)

const { status, data } = await apiInstance.listCartItems(
    cname,
    lang
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **cname** | [**string**] | Customer name | (optional) defaults to undefined|
| **lang** | [**string**] | Response language | (optional) defaults to undefined|


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
|**200** | Cart item list response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **updateCartItem**
> CreateDnsRecord200Response updateCartItem(updateCartItemRequest)


### Example

```typescript
import {
    CartApi,
    Configuration,
    UpdateCartItemRequest
} from '@platon-net/cp-typescript-sdk';

const configuration = new Configuration();
const apiInstance = new CartApi(configuration);

let cartItemId: number; //Cart item ID (default to undefined)
let updateCartItemRequest: UpdateCartItemRequest; //Cart item update payload

const { status, data } = await apiInstance.updateCartItem(
    cartItemId,
    updateCartItemRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **updateCartItemRequest** | **UpdateCartItemRequest**| Cart item update payload | |
| **cartItemId** | [**number**] | Cart item ID | defaults to undefined|


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
|**200** | Cart item update response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **updateCartItemCount**
> CreateDnsRecord200Response updateCartItemCount(updateCartItemCountRequest)


### Example

```typescript
import {
    CartApi,
    Configuration,
    UpdateCartItemCountRequest
} from '@platon-net/cp-typescript-sdk';

const configuration = new Configuration();
const apiInstance = new CartApi(configuration);

let updateCartItemCountRequest: UpdateCartItemCountRequest; //Cart item count update payload

const { status, data } = await apiInstance.updateCartItemCount(
    updateCartItemCountRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **updateCartItemCountRequest** | **UpdateCartItemCountRequest**| Cart item count update payload | |


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
|**200** | Cart item count update response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

