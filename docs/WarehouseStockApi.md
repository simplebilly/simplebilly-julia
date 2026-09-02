# WarehouseStockApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_warehouse_stock**](WarehouseStockApi.md#create_warehouse_stock) | **POST** /api/v1/warehouses/{warehouse_id}/stock | 
[**delete_warehouse_stock**](WarehouseStockApi.md#delete_warehouse_stock) | **DELETE** /api/v1/warehouses/{warehouse_id}/stock/{product_id} | 
[**list_warehouse_stock**](WarehouseStockApi.md#list_warehouse_stock) | **GET** /api/v1/warehouses/{warehouse_id}/stock | 
[**update_warehouse_stock**](WarehouseStockApi.md#update_warehouse_stock) | **PUT** /api/v1/warehouses/{warehouse_id}/stock/{product_id} | 


# **create_warehouse_stock**
> `create_warehouse_stock`(_api::`WarehouseStockApi`, `warehouse_id`::`String`, `stock_adjustment`::`StockAdjustment`; _mediaType=nothing) -> `WarehouseStock`, `OpenAPI.Clients.ApiResponse` <br/>
> `create_warehouse_stock`(_api::`WarehouseStockApi`, response_stream::`Channel`, `warehouse_id`::`String`, `stock_adjustment`::`StockAdjustment`; _mediaType=nothing) -> `Channel`{ `WarehouseStock` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`WarehouseStockApi`** | API context | 
**`warehouse_id`** | **`String`** |  |
**`stock_adjustment`** | [**`StockAdjustment`**](StockAdjustment.md) |  |

### Return type

[**`WarehouseStock`**](WarehouseStock.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **delete_warehouse_stock**
> `delete_warehouse_stock`(_api::`WarehouseStockApi`, `warehouse_id`::`String`, `product_id`::`String`; _mediaType=nothing) -> `Nothing`, `OpenAPI.Clients.ApiResponse` <br/>
> `delete_warehouse_stock`(_api::`WarehouseStockApi`, response_stream::`Channel`, `warehouse_id`::`String`, `product_id`::`String`; _mediaType=nothing) -> `Channel`{ `Nothing` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`WarehouseStockApi`** | API context | 
**`warehouse_id`** | **`String`** |  |
**`product_id`** | **`String`** |  |

### Return type

`Nothing`

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **list_warehouse_stock**
> `list_warehouse_stock`(_api::`WarehouseStockApi`, `warehouse_id`::`String`; _mediaType=nothing) -> `Vector{WarehouseStock}`, `OpenAPI.Clients.ApiResponse` <br/>
> `list_warehouse_stock`(_api::`WarehouseStockApi`, response_stream::`Channel`, `warehouse_id`::`String`; _mediaType=nothing) -> `Channel`{ `Vector{WarehouseStock}` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`WarehouseStockApi`** | API context | 
**`warehouse_id`** | **`String`** |  |

### Return type

[**`Vector{WarehouseStock}`**](WarehouseStock.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **update_warehouse_stock**
> `update_warehouse_stock`(_api::`WarehouseStockApi`, `warehouse_id`::`String`, `product_id`::`String`, `stock_adjustment`::`StockAdjustment`; _mediaType=nothing) -> `WarehouseStock`, `OpenAPI.Clients.ApiResponse` <br/>
> `update_warehouse_stock`(_api::`WarehouseStockApi`, response_stream::`Channel`, `warehouse_id`::`String`, `product_id`::`String`, `stock_adjustment`::`StockAdjustment`; _mediaType=nothing) -> `Channel`{ `WarehouseStock` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`WarehouseStockApi`** | API context | 
**`warehouse_id`** | **`String`** |  |
**`product_id`** | **`String`** |  |
**`stock_adjustment`** | [**`StockAdjustment`**](StockAdjustment.md) |  |

### Return type

[**`WarehouseStock`**](WarehouseStock.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

