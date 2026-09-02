# ProductionOrderApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_production_order**](ProductionOrderApi.md#create_production_order) | **POST** /api/v1/production-orders | 
[**delete_production_order**](ProductionOrderApi.md#delete_production_order) | **DELETE** /api/v1/production-orders/{production_order_id} | 
[**get_production_order**](ProductionOrderApi.md#get_production_order) | **GET** /api/v1/production-orders/{production_order_id} | 
[**list_production_orders**](ProductionOrderApi.md#list_production_orders) | **GET** /api/v1/production-orders/ | 
[**production_order_costing**](ProductionOrderApi.md#production_order_costing) | **GET** /api/v1/production-orders/{production_order_id}/costing | Actual-costing report (Nachkalkulation) — material costs from BOM components at their purchase price plus the resulting per-unit cost and margin against the finished product&#39;s sale price.
[**update_production_order**](ProductionOrderApi.md#update_production_order) | **PUT** /api/v1/production-orders/{production_order_id} | 
[**update_production_order_status**](ProductionOrderApi.md#update_production_order_status) | **PUT** /api/v1/production-orders/{production_order_id}/status | 


# **create_production_order**
> `create_production_order`(_api::`ProductionOrderApi`, `production_order`::`ProductionOrder`; _mediaType=nothing) -> `ProductionOrder`, `OpenAPI.Clients.ApiResponse` <br/>
> `create_production_order`(_api::`ProductionOrderApi`, response_stream::`Channel`, `production_order`::`ProductionOrder`; _mediaType=nothing) -> `Channel`{ `ProductionOrder` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ProductionOrderApi`** | API context | 
**`production_order`** | [**`ProductionOrder`**](ProductionOrder.md) |  |

### Return type

[**`ProductionOrder`**](ProductionOrder.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **delete_production_order**
> `delete_production_order`(_api::`ProductionOrderApi`, `production_order_id`::`String`; _mediaType=nothing) -> `Nothing`, `OpenAPI.Clients.ApiResponse` <br/>
> `delete_production_order`(_api::`ProductionOrderApi`, response_stream::`Channel`, `production_order_id`::`String`; _mediaType=nothing) -> `Channel`{ `Nothing` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ProductionOrderApi`** | API context | 
**`production_order_id`** | **`String`** |  |

### Return type

`Nothing`

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **get_production_order**
> `get_production_order`(_api::`ProductionOrderApi`, `production_order_id`::`String`; _mediaType=nothing) -> `ProductionOrder`, `OpenAPI.Clients.ApiResponse` <br/>
> `get_production_order`(_api::`ProductionOrderApi`, response_stream::`Channel`, `production_order_id`::`String`; _mediaType=nothing) -> `Channel`{ `ProductionOrder` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ProductionOrderApi`** | API context | 
**`production_order_id`** | **`String`** |  |

### Return type

[**`ProductionOrder`**](ProductionOrder.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **list_production_orders**
> `list_production_orders`(_api::`ProductionOrderApi`; `page`=nothing, `page_size`=nothing, `search`=nothing, `status`=nothing, _mediaType=nothing) -> `Vector{ProductionOrder}`, `OpenAPI.Clients.ApiResponse` <br/>
> `list_production_orders`(_api::`ProductionOrderApi`, response_stream::`Channel`; `page`=nothing, `page_size`=nothing, `search`=nothing, `status`=nothing, _mediaType=nothing) -> `Channel`{ `Vector{ProductionOrder}` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ProductionOrderApi`** | API context | 

### Optional Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **`page`** | **`Int64`** |  | [default to nothing]
 **`page_size`** | **`Int64`** |  | [default to nothing]
 **`search`** | **`String`** |  | [default to nothing]
 **`status`** | **`String`** | Filter by status. | [default to nothing]

### Return type

[**`Vector{ProductionOrder}`**](ProductionOrder.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **production_order_costing**
> `production_order_costing`(_api::`ProductionOrderApi`, `production_order_id`::`String`; _mediaType=nothing) -> `ProductionOrderCosting`, `OpenAPI.Clients.ApiResponse` <br/>
> `production_order_costing`(_api::`ProductionOrderApi`, response_stream::`Channel`, `production_order_id`::`String`; _mediaType=nothing) -> `Channel`{ `ProductionOrderCosting` }, `OpenAPI.Clients.ApiResponse`

Actual-costing report (Nachkalkulation) — material costs from BOM components at their purchase price plus the resulting per-unit cost and margin against the finished product's sale price.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ProductionOrderApi`** | API context | 
**`production_order_id`** | **`String`** |  |

### Return type

[**`ProductionOrderCosting`**](ProductionOrderCosting.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **update_production_order**
> `update_production_order`(_api::`ProductionOrderApi`, `production_order_id`::`String`, `production_order`::`ProductionOrder`; _mediaType=nothing) -> `ProductionOrder`, `OpenAPI.Clients.ApiResponse` <br/>
> `update_production_order`(_api::`ProductionOrderApi`, response_stream::`Channel`, `production_order_id`::`String`, `production_order`::`ProductionOrder`; _mediaType=nothing) -> `Channel`{ `ProductionOrder` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ProductionOrderApi`** | API context | 
**`production_order_id`** | **`String`** |  |
**`production_order`** | [**`ProductionOrder`**](ProductionOrder.md) |  |

### Return type

[**`ProductionOrder`**](ProductionOrder.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **update_production_order_status**
> `update_production_order_status`(_api::`ProductionOrderApi`, `production_order_id`::`String`, `production_order_status_update`::`ProductionOrderStatusUpdate`; _mediaType=nothing) -> `ProductionOrder`, `OpenAPI.Clients.ApiResponse` <br/>
> `update_production_order_status`(_api::`ProductionOrderApi`, response_stream::`Channel`, `production_order_id`::`String`, `production_order_status_update`::`ProductionOrderStatusUpdate`; _mediaType=nothing) -> `Channel`{ `ProductionOrder` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ProductionOrderApi`** | API context | 
**`production_order_id`** | **`String`** |  |
**`production_order_status_update`** | [**`ProductionOrderStatusUpdate`**](ProductionOrderStatusUpdate.md) |  |

### Return type

[**`ProductionOrder`**](ProductionOrder.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

