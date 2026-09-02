# StockMovementApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_stock_movement**](StockMovementApi.md#get_stock_movement) | **GET** /api/v1/stock-movements/{movement_id} | 
[**list_stock_movements**](StockMovementApi.md#list_stock_movements) | **GET** /api/v1/stock-movements/ | 


# **get_stock_movement**
> `get_stock_movement`(_api::`StockMovementApi`, `movement_id`::`String`; _mediaType=nothing) -> `StockMovement`, `OpenAPI.Clients.ApiResponse` <br/>
> `get_stock_movement`(_api::`StockMovementApi`, response_stream::`Channel`, `movement_id`::`String`; _mediaType=nothing) -> `Channel`{ `StockMovement` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`StockMovementApi`** | API context | 
**`movement_id`** | **`String`** |  |

### Return type

[**`StockMovement`**](StockMovement.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **list_stock_movements**
> `list_stock_movements`(_api::`StockMovementApi`; `page`=nothing, `page_size`=nothing, `product_id`=nothing, `warehouse_id`=nothing, `movement_type`=nothing, `from`=nothing, `to`=nothing, _mediaType=nothing) -> `Vector{StockMovement}`, `OpenAPI.Clients.ApiResponse` <br/>
> `list_stock_movements`(_api::`StockMovementApi`, response_stream::`Channel`; `page`=nothing, `page_size`=nothing, `product_id`=nothing, `warehouse_id`=nothing, `movement_type`=nothing, `from`=nothing, `to`=nothing, _mediaType=nothing) -> `Channel`{ `Vector{StockMovement}` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`StockMovementApi`** | API context | 

### Optional Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **`page`** | **`Int64`** |  | [default to nothing]
 **`page_size`** | **`Int64`** |  | [default to nothing]
 **`product_id`** | **`String`** |  | [default to nothing]
 **`warehouse_id`** | **`String`** |  | [default to nothing]
 **`movement_type`** | **`String`** |  | [default to nothing]
 **`from`** | **`Date`** | Only movements on or after this date (inclusive). | [default to nothing]
 **`to`** | **`Date`** | Only movements on or before this date (inclusive). | [default to nothing]

### Return type

[**`Vector{StockMovement}`**](StockMovement.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

