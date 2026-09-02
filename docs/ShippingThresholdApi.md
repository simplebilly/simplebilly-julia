# ShippingThresholdApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_shipping_threshold**](ShippingThresholdApi.md#create_shipping_threshold) | **POST** /api/v1/shipping-thresholds | 
[**delete_shipping_threshold**](ShippingThresholdApi.md#delete_shipping_threshold) | **DELETE** /api/v1/shipping-thresholds/{threshold_id} | 
[**get_deliverable**](ShippingThresholdApi.md#get_deliverable) | **GET** /api/v1/shipping-thresholds/deliverable | 
[**get_shipping_threshold**](ShippingThresholdApi.md#get_shipping_threshold) | **GET** /api/v1/shipping-thresholds/{threshold_id} | 
[**list_shipping_thresholds**](ShippingThresholdApi.md#list_shipping_thresholds) | **GET** /api/v1/shipping-thresholds/ | 
[**update_shipping_threshold**](ShippingThresholdApi.md#update_shipping_threshold) | **PUT** /api/v1/shipping-thresholds/{threshold_id} | 


# **create_shipping_threshold**
> `create_shipping_threshold`(_api::`ShippingThresholdApi`, `shipping_threshold_create`::`ShippingThresholdCreate`; _mediaType=nothing) -> `ShippingThreshold`, `OpenAPI.Clients.ApiResponse` <br/>
> `create_shipping_threshold`(_api::`ShippingThresholdApi`, response_stream::`Channel`, `shipping_threshold_create`::`ShippingThresholdCreate`; _mediaType=nothing) -> `Channel`{ `ShippingThreshold` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ShippingThresholdApi`** | API context | 
**`shipping_threshold_create`** | [**`ShippingThresholdCreate`**](ShippingThresholdCreate.md) |  |

### Return type

[**`ShippingThreshold`**](ShippingThreshold.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **delete_shipping_threshold**
> `delete_shipping_threshold`(_api::`ShippingThresholdApi`, `threshold_id`::`String`; _mediaType=nothing) -> `Nothing`, `OpenAPI.Clients.ApiResponse` <br/>
> `delete_shipping_threshold`(_api::`ShippingThresholdApi`, response_stream::`Channel`, `threshold_id`::`String`; _mediaType=nothing) -> `Channel`{ `Nothing` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ShippingThresholdApi`** | API context | 
**`threshold_id`** | **`String`** |  |

### Return type

`Nothing`

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **get_deliverable**
> `get_deliverable`(_api::`ShippingThresholdApi`, `product_id`::`String`; `warehouse_id`=nothing, _mediaType=nothing) -> `DeliverableResponse`, `OpenAPI.Clients.ApiResponse` <br/>
> `get_deliverable`(_api::`ShippingThresholdApi`, response_stream::`Channel`, `product_id`::`String`; `warehouse_id`=nothing, _mediaType=nothing) -> `Channel`{ `DeliverableResponse` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ShippingThresholdApi`** | API context | 
**`product_id`** | **`String`** |  |

### Optional Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **`warehouse_id`** | **`String`** |  | [default to nothing]

### Return type

[**`DeliverableResponse`**](DeliverableResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **get_shipping_threshold**
> `get_shipping_threshold`(_api::`ShippingThresholdApi`, `threshold_id`::`String`; _mediaType=nothing) -> `ShippingThreshold`, `OpenAPI.Clients.ApiResponse` <br/>
> `get_shipping_threshold`(_api::`ShippingThresholdApi`, response_stream::`Channel`, `threshold_id`::`String`; _mediaType=nothing) -> `Channel`{ `ShippingThreshold` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ShippingThresholdApi`** | API context | 
**`threshold_id`** | **`String`** |  |

### Return type

[**`ShippingThreshold`**](ShippingThreshold.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **list_shipping_thresholds**
> `list_shipping_thresholds`(_api::`ShippingThresholdApi`; `page`=nothing, `page_size`=nothing, `product_id`=nothing, `warehouse_id`=nothing, `is_active`=nothing, _mediaType=nothing) -> `Vector{ShippingThreshold}`, `OpenAPI.Clients.ApiResponse` <br/>
> `list_shipping_thresholds`(_api::`ShippingThresholdApi`, response_stream::`Channel`; `page`=nothing, `page_size`=nothing, `product_id`=nothing, `warehouse_id`=nothing, `is_active`=nothing, _mediaType=nothing) -> `Channel`{ `Vector{ShippingThreshold}` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ShippingThresholdApi`** | API context | 

### Optional Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **`page`** | **`Int64`** |  | [default to nothing]
 **`page_size`** | **`Int64`** |  | [default to nothing]
 **`product_id`** | **`String`** |  | [default to nothing]
 **`warehouse_id`** | **`String`** |  | [default to nothing]
 **`is_active`** | **`Bool`** |  | [default to nothing]

### Return type

[**`Vector{ShippingThreshold}`**](ShippingThreshold.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **update_shipping_threshold**
> `update_shipping_threshold`(_api::`ShippingThresholdApi`, `threshold_id`::`String`, `shipping_threshold_update`::`ShippingThresholdUpdate`; _mediaType=nothing) -> `ShippingThreshold`, `OpenAPI.Clients.ApiResponse` <br/>
> `update_shipping_threshold`(_api::`ShippingThresholdApi`, response_stream::`Channel`, `threshold_id`::`String`, `shipping_threshold_update`::`ShippingThresholdUpdate`; _mediaType=nothing) -> `Channel`{ `ShippingThreshold` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ShippingThresholdApi`** | API context | 
**`threshold_id`** | **`String`** |  |
**`shipping_threshold_update`** | [**`ShippingThresholdUpdate`**](ShippingThresholdUpdate.md) |  |

### Return type

[**`ShippingThreshold`**](ShippingThreshold.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

