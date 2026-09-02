# StockTransferApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_stock_transfer**](StockTransferApi.md#create_stock_transfer) | **POST** /api/v1/stock-transfers | 
[**delete_stock_transfer**](StockTransferApi.md#delete_stock_transfer) | **DELETE** /api/v1/stock-transfers/{stock_transfer_id} | 
[**get_stock_transfer**](StockTransferApi.md#get_stock_transfer) | **GET** /api/v1/stock-transfers/{stock_transfer_id} | 
[**list_stock_transfers**](StockTransferApi.md#list_stock_transfers) | **GET** /api/v1/stock-transfers/ | 
[**update_stock_transfer_status**](StockTransferApi.md#update_stock_transfer_status) | **PUT** /api/v1/stock-transfers/{stock_transfer_id}/status | 


# **create_stock_transfer**
> `create_stock_transfer`(_api::`StockTransferApi`, `stock_transfer`::`StockTransfer`; _mediaType=nothing) -> `StockTransfer`, `OpenAPI.Clients.ApiResponse` <br/>
> `create_stock_transfer`(_api::`StockTransferApi`, response_stream::`Channel`, `stock_transfer`::`StockTransfer`; _mediaType=nothing) -> `Channel`{ `StockTransfer` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`StockTransferApi`** | API context | 
**`stock_transfer`** | [**`StockTransfer`**](StockTransfer.md) |  |

### Return type

[**`StockTransfer`**](StockTransfer.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **delete_stock_transfer**
> `delete_stock_transfer`(_api::`StockTransferApi`, `stock_transfer_id`::`String`; _mediaType=nothing) -> `Nothing`, `OpenAPI.Clients.ApiResponse` <br/>
> `delete_stock_transfer`(_api::`StockTransferApi`, response_stream::`Channel`, `stock_transfer_id`::`String`; _mediaType=nothing) -> `Channel`{ `Nothing` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`StockTransferApi`** | API context | 
**`stock_transfer_id`** | **`String`** |  |

### Return type

`Nothing`

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **get_stock_transfer**
> `get_stock_transfer`(_api::`StockTransferApi`, `stock_transfer_id`::`String`; _mediaType=nothing) -> `StockTransfer`, `OpenAPI.Clients.ApiResponse` <br/>
> `get_stock_transfer`(_api::`StockTransferApi`, response_stream::`Channel`, `stock_transfer_id`::`String`; _mediaType=nothing) -> `Channel`{ `StockTransfer` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`StockTransferApi`** | API context | 
**`stock_transfer_id`** | **`String`** |  |

### Return type

[**`StockTransfer`**](StockTransfer.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **list_stock_transfers**
> `list_stock_transfers`(_api::`StockTransferApi`; `page`=nothing, `page_size`=nothing, `status`=nothing, `warehouse_id`=nothing, _mediaType=nothing) -> `Vector{StockTransfer}`, `OpenAPI.Clients.ApiResponse` <br/>
> `list_stock_transfers`(_api::`StockTransferApi`, response_stream::`Channel`; `page`=nothing, `page_size`=nothing, `status`=nothing, `warehouse_id`=nothing, _mediaType=nothing) -> `Channel`{ `Vector{StockTransfer}` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`StockTransferApi`** | API context | 

### Optional Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **`page`** | **`Int64`** |  | [default to nothing]
 **`page_size`** | **`Int64`** |  | [default to nothing]
 **`status`** | **`String`** |  | [default to nothing]
 **`warehouse_id`** | **`String`** |  | [default to nothing]

### Return type

[**`Vector{StockTransfer}`**](StockTransfer.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **update_stock_transfer_status**
> `update_stock_transfer_status`(_api::`StockTransferApi`, `stock_transfer_id`::`String`, `stock_transfer_status_update`::`StockTransferStatusUpdate`; _mediaType=nothing) -> `StockTransfer`, `OpenAPI.Clients.ApiResponse` <br/>
> `update_stock_transfer_status`(_api::`StockTransferApi`, response_stream::`Channel`, `stock_transfer_id`::`String`, `stock_transfer_status_update`::`StockTransferStatusUpdate`; _mediaType=nothing) -> `Channel`{ `StockTransfer` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`StockTransferApi`** | API context | 
**`stock_transfer_id`** | **`String`** |  |
**`stock_transfer_status_update`** | [**`StockTransferStatusUpdate`**](StockTransferStatusUpdate.md) |  |

### Return type

[**`StockTransfer`**](StockTransfer.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

