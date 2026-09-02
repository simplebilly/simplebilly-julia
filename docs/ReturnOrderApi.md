# ReturnOrderApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_return_order**](ReturnOrderApi.md#create_return_order) | **POST** /api/v1/returns | 
[**delete_return_order**](ReturnOrderApi.md#delete_return_order) | **DELETE** /api/v1/returns/{return_order_id} | 
[**get_return_order**](ReturnOrderApi.md#get_return_order) | **GET** /api/v1/returns/{return_order_id} | 
[**list_return_orders**](ReturnOrderApi.md#list_return_orders) | **GET** /api/v1/returns/ | 
[**return_logistics_queue**](ReturnOrderApi.md#return_logistics_queue) | **GET** /api/v1/returns/logistics-queue | 
[**return_logistics_summary**](ReturnOrderApi.md#return_logistics_summary) | **GET** /api/v1/returns/logistics-summary | Returns-logistics aggregation for the dashboard: quantities received, restocked and scrapped per warehouse.
[**update_return_order**](ReturnOrderApi.md#update_return_order) | **PUT** /api/v1/returns/{return_order_id} | 
[**update_return_order_status**](ReturnOrderApi.md#update_return_order_status) | **PUT** /api/v1/returns/{return_order_id}/status | 


# **create_return_order**
> `create_return_order`(_api::`ReturnOrderApi`, `return_order`::`ReturnOrder`; _mediaType=nothing) -> `ReturnOrder`, `OpenAPI.Clients.ApiResponse` <br/>
> `create_return_order`(_api::`ReturnOrderApi`, response_stream::`Channel`, `return_order`::`ReturnOrder`; _mediaType=nothing) -> `Channel`{ `ReturnOrder` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ReturnOrderApi`** | API context | 
**`return_order`** | [**`ReturnOrder`**](ReturnOrder.md) |  |

### Return type

[**`ReturnOrder`**](ReturnOrder.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **delete_return_order**
> `delete_return_order`(_api::`ReturnOrderApi`, `return_order_id`::`String`; _mediaType=nothing) -> `Nothing`, `OpenAPI.Clients.ApiResponse` <br/>
> `delete_return_order`(_api::`ReturnOrderApi`, response_stream::`Channel`, `return_order_id`::`String`; _mediaType=nothing) -> `Channel`{ `Nothing` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ReturnOrderApi`** | API context | 
**`return_order_id`** | **`String`** |  |

### Return type

`Nothing`

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **get_return_order**
> `get_return_order`(_api::`ReturnOrderApi`, `return_order_id`::`String`; _mediaType=nothing) -> `ReturnOrder`, `OpenAPI.Clients.ApiResponse` <br/>
> `get_return_order`(_api::`ReturnOrderApi`, response_stream::`Channel`, `return_order_id`::`String`; _mediaType=nothing) -> `Channel`{ `ReturnOrder` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ReturnOrderApi`** | API context | 
**`return_order_id`** | **`String`** |  |

### Return type

[**`ReturnOrder`**](ReturnOrder.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **list_return_orders**
> `list_return_orders`(_api::`ReturnOrderApi`; `page`=nothing, `page_size`=nothing, `status`=nothing, `customer_name`=nothing, `order_number`=nothing, _mediaType=nothing) -> `Vector{ReturnOrder}`, `OpenAPI.Clients.ApiResponse` <br/>
> `list_return_orders`(_api::`ReturnOrderApi`, response_stream::`Channel`; `page`=nothing, `page_size`=nothing, `status`=nothing, `customer_name`=nothing, `order_number`=nothing, _mediaType=nothing) -> `Channel`{ `Vector{ReturnOrder}` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ReturnOrderApi`** | API context | 

### Optional Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **`page`** | **`Int64`** |  | [default to nothing]
 **`page_size`** | **`Int64`** |  | [default to nothing]
 **`status`** | **`String`** |  | [default to nothing]
 **`customer_name`** | **`String`** |  | [default to nothing]
 **`order_number`** | **`String`** |  | [default to nothing]

### Return type

[**`Vector{ReturnOrder}`**](ReturnOrder.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **return_logistics_queue**
> `return_logistics_queue`(_api::`ReturnOrderApi`; _mediaType=nothing) -> `Vector{ReturnLogisticsQueueItem}`, `OpenAPI.Clients.ApiResponse` <br/>
> `return_logistics_queue`(_api::`ReturnOrderApi`, response_stream::`Channel`; _mediaType=nothing) -> `Channel`{ `Vector{ReturnLogisticsQueueItem}` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters
This endpoint does not need any parameter.

### Return type

[**`Vector{ReturnLogisticsQueueItem}`**](ReturnLogisticsQueueItem.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **return_logistics_summary**
> `return_logistics_summary`(_api::`ReturnOrderApi`; _mediaType=nothing) -> `ReturnLogisticsSummary`, `OpenAPI.Clients.ApiResponse` <br/>
> `return_logistics_summary`(_api::`ReturnOrderApi`, response_stream::`Channel`; _mediaType=nothing) -> `Channel`{ `ReturnLogisticsSummary` }, `OpenAPI.Clients.ApiResponse`

Returns-logistics aggregation for the dashboard: quantities received, restocked and scrapped per warehouse.

### Required Parameters
This endpoint does not need any parameter.

### Return type

[**`ReturnLogisticsSummary`**](ReturnLogisticsSummary.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **update_return_order**
> `update_return_order`(_api::`ReturnOrderApi`, `return_order_id`::`String`, `body`::`Any`; _mediaType=nothing) -> `ReturnOrder`, `OpenAPI.Clients.ApiResponse` <br/>
> `update_return_order`(_api::`ReturnOrderApi`, response_stream::`Channel`, `return_order_id`::`String`, `body`::`Any`; _mediaType=nothing) -> `Channel`{ `ReturnOrder` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ReturnOrderApi`** | API context | 
**`return_order_id`** | **`String`** |  |
**`body`** | **`Any`** |  |

### Return type

[**`ReturnOrder`**](ReturnOrder.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **update_return_order_status**
> `update_return_order_status`(_api::`ReturnOrderApi`, `return_order_id`::`String`, `return_order_status_update`::`ReturnOrderStatusUpdate`; _mediaType=nothing) -> `ReturnOrder`, `OpenAPI.Clients.ApiResponse` <br/>
> `update_return_order_status`(_api::`ReturnOrderApi`, response_stream::`Channel`, `return_order_id`::`String`, `return_order_status_update`::`ReturnOrderStatusUpdate`; _mediaType=nothing) -> `Channel`{ `ReturnOrder` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ReturnOrderApi`** | API context | 
**`return_order_id`** | **`String`** |  |
**`return_order_status_update`** | [**`ReturnOrderStatusUpdate`**](ReturnOrderStatusUpdate.md) |  |

### Return type

[**`ReturnOrder`**](ReturnOrder.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

