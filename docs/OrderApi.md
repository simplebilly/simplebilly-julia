# OrderApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**add_order_tags**](OrderApi.md#add_order_tags) | **POST** /api/v1/orders/{order_id}/tags | 
[**find_order_by_external_ref**](OrderApi.md#find_order_by_external_ref) | **GET** /api/v1/orders/by-ext-ref/{ext_ref} | 
[**get_order**](OrderApi.md#get_order) | **GET** /api/v1/order/{order_number} | 
[**get_orders**](OrderApi.md#get_orders) | **GET** /api/v1/orders | 
[**patch_order**](OrderApi.md#patch_order) | **PATCH** /api/v1/orders/{order_id} | 
[**replace_order_tags**](OrderApi.md#replace_order_tags) | **PUT** /api/v1/orders/{order_id}/tags | 
[**update_order_state**](OrderApi.md#update_order_state) | **PUT** /api/v1/orders/{order_id}/state | 


# **add_order_tags**
> `add_order_tags`(_api::`OrderApi`, `order_id`::`String`, `order_tags_request`::`OrderTagsRequest`; _mediaType=nothing) -> `Order`, `OpenAPI.Clients.ApiResponse` <br/>
> `add_order_tags`(_api::`OrderApi`, response_stream::`Channel`, `order_id`::`String`, `order_tags_request`::`OrderTagsRequest`; _mediaType=nothing) -> `Channel`{ `Order` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`OrderApi`** | API context | 
**`order_id`** | **`String`** |  |
**`order_tags_request`** | [**`OrderTagsRequest`**](OrderTagsRequest.md) |  |

### Return type

[**`Order`**](Order.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **find_order_by_external_ref**
> `find_order_by_external_ref`(_api::`OrderApi`, `ext_ref`::`String`; _mediaType=nothing) -> `Order`, `OpenAPI.Clients.ApiResponse` <br/>
> `find_order_by_external_ref`(_api::`OrderApi`, response_stream::`Channel`, `ext_ref`::`String`; _mediaType=nothing) -> `Channel`{ `Order` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`OrderApi`** | API context | 
**`ext_ref`** | **`String`** |  |

### Return type

[**`Order`**](Order.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **get_order**
> `get_order`(_api::`OrderApi`, `order_number`::`String`; _mediaType=nothing) -> `Order`, `OpenAPI.Clients.ApiResponse` <br/>
> `get_order`(_api::`OrderApi`, response_stream::`Channel`, `order_number`::`String`; _mediaType=nothing) -> `Channel`{ `Order` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`OrderApi`** | API context | 
**`order_number`** | **`String`** |  |

### Return type

[**`Order`**](Order.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **get_orders**
> `get_orders`(_api::`OrderApi`; `page`=nothing, `page_size`=nothing, `search`=nothing, `include_deleted`=nothing, _mediaType=nothing) -> `Vector{Order}`, `OpenAPI.Clients.ApiResponse` <br/>
> `get_orders`(_api::`OrderApi`, response_stream::`Channel`; `page`=nothing, `page_size`=nothing, `search`=nothing, `include_deleted`=nothing, _mediaType=nothing) -> `Channel`{ `Vector{Order}` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`OrderApi`** | API context | 

### Optional Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **`page`** | **`Int64`** |  | [default to nothing]
 **`page_size`** | **`Int64`** |  | [default to nothing]
 **`search`** | **`String`** |  | [default to nothing]
 **`include_deleted`** | **`Bool`** | Soft-delete entities: set true to include rows with &#x60;deleted_at&#x60; set. | [default to nothing]

### Return type

[**`Vector{Order}`**](Order.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **patch_order**
> `patch_order`(_api::`OrderApi`, `order_id`::`String`, `body`::`Any`; _mediaType=nothing) -> `Order`, `OpenAPI.Clients.ApiResponse` <br/>
> `patch_order`(_api::`OrderApi`, response_stream::`Channel`, `order_id`::`String`, `body`::`Any`; _mediaType=nothing) -> `Channel`{ `Order` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`OrderApi`** | API context | 
**`order_id`** | **`String`** |  |
**`body`** | **`Any`** |  |

### Return type

[**`Order`**](Order.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **replace_order_tags**
> `replace_order_tags`(_api::`OrderApi`, `order_id`::`String`, `order_tags_request`::`OrderTagsRequest`; _mediaType=nothing) -> `Order`, `OpenAPI.Clients.ApiResponse` <br/>
> `replace_order_tags`(_api::`OrderApi`, response_stream::`Channel`, `order_id`::`String`, `order_tags_request`::`OrderTagsRequest`; _mediaType=nothing) -> `Channel`{ `Order` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`OrderApi`** | API context | 
**`order_id`** | **`String`** |  |
**`order_tags_request`** | [**`OrderTagsRequest`**](OrderTagsRequest.md) |  |

### Return type

[**`Order`**](Order.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **update_order_state**
> `update_order_state`(_api::`OrderApi`, `order_id`::`String`, `order_state_update`::`OrderStateUpdate`; _mediaType=nothing) -> `Order`, `OpenAPI.Clients.ApiResponse` <br/>
> `update_order_state`(_api::`OrderApi`, response_stream::`Channel`, `order_id`::`String`, `order_state_update`::`OrderStateUpdate`; _mediaType=nothing) -> `Channel`{ `Order` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`OrderApi`** | API context | 
**`order_id`** | **`String`** |  |
**`order_state_update`** | [**`OrderStateUpdate`**](OrderStateUpdate.md) |  |

### Return type

[**`Order`**](Order.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

