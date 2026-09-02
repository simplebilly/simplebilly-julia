# WarehouseApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_warehouse**](WarehouseApi.md#create_warehouse) | **POST** /api/v1/warehouses | 
[**delete_warehouse**](WarehouseApi.md#delete_warehouse) | **DELETE** /api/v1/warehouses/{warehouse_id} | 
[**get_warehouse**](WarehouseApi.md#get_warehouse) | **GET** /api/v1/warehouses/{warehouse_id} | 
[**list_warehouses**](WarehouseApi.md#list_warehouses) | **GET** /api/v1/warehouses/ | 
[**update_warehouse**](WarehouseApi.md#update_warehouse) | **PUT** /api/v1/warehouses/{warehouse_id} | 


# **create_warehouse**
> `create_warehouse`(_api::`WarehouseApi`, `warehouse`::`Warehouse`; _mediaType=nothing) -> `Warehouse`, `OpenAPI.Clients.ApiResponse` <br/>
> `create_warehouse`(_api::`WarehouseApi`, response_stream::`Channel`, `warehouse`::`Warehouse`; _mediaType=nothing) -> `Channel`{ `Warehouse` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`WarehouseApi`** | API context | 
**`warehouse`** | [**`Warehouse`**](Warehouse.md) |  |

### Return type

[**`Warehouse`**](Warehouse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **delete_warehouse**
> `delete_warehouse`(_api::`WarehouseApi`, `warehouse_id`::`String`; _mediaType=nothing) -> `Nothing`, `OpenAPI.Clients.ApiResponse` <br/>
> `delete_warehouse`(_api::`WarehouseApi`, response_stream::`Channel`, `warehouse_id`::`String`; _mediaType=nothing) -> `Channel`{ `Nothing` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`WarehouseApi`** | API context | 
**`warehouse_id`** | **`String`** |  |

### Return type

`Nothing`

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **get_warehouse**
> `get_warehouse`(_api::`WarehouseApi`, `warehouse_id`::`String`; _mediaType=nothing) -> `Warehouse`, `OpenAPI.Clients.ApiResponse` <br/>
> `get_warehouse`(_api::`WarehouseApi`, response_stream::`Channel`, `warehouse_id`::`String`; _mediaType=nothing) -> `Channel`{ `Warehouse` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`WarehouseApi`** | API context | 
**`warehouse_id`** | **`String`** |  |

### Return type

[**`Warehouse`**](Warehouse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **list_warehouses**
> `list_warehouses`(_api::`WarehouseApi`; `page`=nothing, `page_size`=nothing, `search`=nothing, `is_active`=nothing, _mediaType=nothing) -> `Vector{Warehouse}`, `OpenAPI.Clients.ApiResponse` <br/>
> `list_warehouses`(_api::`WarehouseApi`, response_stream::`Channel`; `page`=nothing, `page_size`=nothing, `search`=nothing, `is_active`=nothing, _mediaType=nothing) -> `Channel`{ `Vector{Warehouse}` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`WarehouseApi`** | API context | 

### Optional Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **`page`** | **`Int64`** |  | [default to nothing]
 **`page_size`** | **`Int64`** |  | [default to nothing]
 **`search`** | **`String`** |  | [default to nothing]
 **`is_active`** | **`Bool`** |  | [default to nothing]

### Return type

[**`Vector{Warehouse}`**](Warehouse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **update_warehouse**
> `update_warehouse`(_api::`WarehouseApi`, `warehouse_id`::`String`, `body`::`Any`; _mediaType=nothing) -> `Warehouse`, `OpenAPI.Clients.ApiResponse` <br/>
> `update_warehouse`(_api::`WarehouseApi`, response_stream::`Channel`, `warehouse_id`::`String`, `body`::`Any`; _mediaType=nothing) -> `Channel`{ `Warehouse` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`WarehouseApi`** | API context | 
**`warehouse_id`** | **`String`** |  |
**`body`** | **`Any`** |  |

### Return type

[**`Warehouse`**](Warehouse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

