# CouponApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**coupon_restore**](CouponApi.md#coupon_restore) | **POST** /api/v1/coupons/{coupon_id}/restore | 
[**create_coupon**](CouponApi.md#create_coupon) | **POST** /api/v1/coupons | 
[**delete_coupon**](CouponApi.md#delete_coupon) | **DELETE** /api/v1/coupons/{coupon_id} | 
[**get_coupon**](CouponApi.md#get_coupon) | **GET** /api/v1/coupons/{coupon_id} | 
[**list_coupons**](CouponApi.md#list_coupons) | **GET** /api/v1/coupons/ | 
[**update_coupon**](CouponApi.md#update_coupon) | **PUT** /api/v1/coupons/{coupon_id} | 


# **coupon_restore**
> `coupon_restore`(_api::`CouponApi`, `coupon_id`::`String`; _mediaType=nothing) -> `Coupon`, `OpenAPI.Clients.ApiResponse` <br/>
> `coupon_restore`(_api::`CouponApi`, response_stream::`Channel`, `coupon_id`::`String`; _mediaType=nothing) -> `Channel`{ `Coupon` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`CouponApi`** | API context | 
**`coupon_id`** | **`String`** |  |

### Return type

[**`Coupon`**](Coupon.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **create_coupon**
> `create_coupon`(_api::`CouponApi`, `coupon_create`::`CouponCreate`; _mediaType=nothing) -> `Coupon`, `OpenAPI.Clients.ApiResponse` <br/>
> `create_coupon`(_api::`CouponApi`, response_stream::`Channel`, `coupon_create`::`CouponCreate`; _mediaType=nothing) -> `Channel`{ `Coupon` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`CouponApi`** | API context | 
**`coupon_create`** | [**`CouponCreate`**](CouponCreate.md) |  |

### Return type

[**`Coupon`**](Coupon.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **delete_coupon**
> `delete_coupon`(_api::`CouponApi`, `coupon_id`::`String`; _mediaType=nothing) -> `Nothing`, `OpenAPI.Clients.ApiResponse` <br/>
> `delete_coupon`(_api::`CouponApi`, response_stream::`Channel`, `coupon_id`::`String`; _mediaType=nothing) -> `Channel`{ `Nothing` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`CouponApi`** | API context | 
**`coupon_id`** | **`String`** |  |

### Return type

`Nothing`

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **get_coupon**
> `get_coupon`(_api::`CouponApi`, `coupon_id`::`String`; _mediaType=nothing) -> `Coupon`, `OpenAPI.Clients.ApiResponse` <br/>
> `get_coupon`(_api::`CouponApi`, response_stream::`Channel`, `coupon_id`::`String`; _mediaType=nothing) -> `Channel`{ `Coupon` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`CouponApi`** | API context | 
**`coupon_id`** | **`String`** |  |

### Return type

[**`Coupon`**](Coupon.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **list_coupons**
> `list_coupons`(_api::`CouponApi`; `page`=nothing, `page_size`=nothing, `is_active`=nothing, `code`=nothing, `discount_type`=nothing, _mediaType=nothing) -> `Vector{Coupon}`, `OpenAPI.Clients.ApiResponse` <br/>
> `list_coupons`(_api::`CouponApi`, response_stream::`Channel`; `page`=nothing, `page_size`=nothing, `is_active`=nothing, `code`=nothing, `discount_type`=nothing, _mediaType=nothing) -> `Channel`{ `Vector{Coupon}` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`CouponApi`** | API context | 

### Optional Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **`page`** | **`Int64`** |  | [default to nothing]
 **`page_size`** | **`Int64`** |  | [default to nothing]
 **`is_active`** | **`Bool`** |  | [default to nothing]
 **`code`** | **`String`** |  | [default to nothing]
 **`discount_type`** | **`String`** |  | [default to nothing]

### Return type

[**`Vector{Coupon}`**](Coupon.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **update_coupon**
> `update_coupon`(_api::`CouponApi`, `coupon_id`::`String`, `coupon_update`::`CouponUpdate`; _mediaType=nothing) -> `Coupon`, `OpenAPI.Clients.ApiResponse` <br/>
> `update_coupon`(_api::`CouponApi`, response_stream::`Channel`, `coupon_id`::`String`, `coupon_update`::`CouponUpdate`; _mediaType=nothing) -> `Channel`{ `Coupon` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`CouponApi`** | API context | 
**`coupon_id`** | **`String`** |  |
**`coupon_update`** | [**`CouponUpdate`**](CouponUpdate.md) |  |

### Return type

[**`Coupon`**](Coupon.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

