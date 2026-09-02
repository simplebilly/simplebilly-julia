# InventoryCountApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_inventory_count**](InventoryCountApi.md#create_inventory_count) | **POST** /api/v1/inventory-counts | 
[**delete_inventory_count**](InventoryCountApi.md#delete_inventory_count) | **DELETE** /api/v1/inventory-counts/{inventory_count_id} | 
[**generate_inventory_count**](InventoryCountApi.md#generate_inventory_count) | **POST** /api/v1/inventory-counts/generate | 
[**get_inventory_count**](InventoryCountApi.md#get_inventory_count) | **GET** /api/v1/inventory-counts/{inventory_count_id} | 
[**list_inventory_counts**](InventoryCountApi.md#list_inventory_counts) | **GET** /api/v1/inventory-counts/ | 
[**update_inventory_count**](InventoryCountApi.md#update_inventory_count) | **PUT** /api/v1/inventory-counts/{inventory_count_id} | 
[**update_inventory_count_status**](InventoryCountApi.md#update_inventory_count_status) | **PUT** /api/v1/inventory-counts/{inventory_count_id}/status | 


# **create_inventory_count**
> `create_inventory_count`(_api::`InventoryCountApi`, `inventory_count`::`InventoryCount`; _mediaType=nothing) -> `InventoryCount`, `OpenAPI.Clients.ApiResponse` <br/>
> `create_inventory_count`(_api::`InventoryCountApi`, response_stream::`Channel`, `inventory_count`::`InventoryCount`; _mediaType=nothing) -> `Channel`{ `InventoryCount` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`InventoryCountApi`** | API context | 
**`inventory_count`** | [**`InventoryCount`**](InventoryCount.md) |  |

### Return type

[**`InventoryCount`**](InventoryCount.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **delete_inventory_count**
> `delete_inventory_count`(_api::`InventoryCountApi`, `inventory_count_id`::`String`; _mediaType=nothing) -> `Nothing`, `OpenAPI.Clients.ApiResponse` <br/>
> `delete_inventory_count`(_api::`InventoryCountApi`, response_stream::`Channel`, `inventory_count_id`::`String`; _mediaType=nothing) -> `Channel`{ `Nothing` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`InventoryCountApi`** | API context | 
**`inventory_count_id`** | **`String`** |  |

### Return type

`Nothing`

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **generate_inventory_count**
> `generate_inventory_count`(_api::`InventoryCountApi`, `generate_count_request`::`GenerateCountRequest`; _mediaType=nothing) -> `InventoryCount`, `OpenAPI.Clients.ApiResponse` <br/>
> `generate_inventory_count`(_api::`InventoryCountApi`, response_stream::`Channel`, `generate_count_request`::`GenerateCountRequest`; _mediaType=nothing) -> `Channel`{ `InventoryCount` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`InventoryCountApi`** | API context | 
**`generate_count_request`** | [**`GenerateCountRequest`**](GenerateCountRequest.md) |  |

### Return type

[**`InventoryCount`**](InventoryCount.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **get_inventory_count**
> `get_inventory_count`(_api::`InventoryCountApi`, `inventory_count_id`::`String`; _mediaType=nothing) -> `InventoryCount`, `OpenAPI.Clients.ApiResponse` <br/>
> `get_inventory_count`(_api::`InventoryCountApi`, response_stream::`Channel`, `inventory_count_id`::`String`; _mediaType=nothing) -> `Channel`{ `InventoryCount` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`InventoryCountApi`** | API context | 
**`inventory_count_id`** | **`String`** |  |

### Return type

[**`InventoryCount`**](InventoryCount.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **list_inventory_counts**
> `list_inventory_counts`(_api::`InventoryCountApi`; `page`=nothing, `page_size`=nothing, `status`=nothing, `warehouse_id`=nothing, _mediaType=nothing) -> `Vector{InventoryCount}`, `OpenAPI.Clients.ApiResponse` <br/>
> `list_inventory_counts`(_api::`InventoryCountApi`, response_stream::`Channel`; `page`=nothing, `page_size`=nothing, `status`=nothing, `warehouse_id`=nothing, _mediaType=nothing) -> `Channel`{ `Vector{InventoryCount}` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`InventoryCountApi`** | API context | 

### Optional Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **`page`** | **`Int64`** |  | [default to nothing]
 **`page_size`** | **`Int64`** |  | [default to nothing]
 **`status`** | **`String`** |  | [default to nothing]
 **`warehouse_id`** | **`String`** |  | [default to nothing]

### Return type

[**`Vector{InventoryCount}`**](InventoryCount.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **update_inventory_count**
> `update_inventory_count`(_api::`InventoryCountApi`, `inventory_count_id`::`String`, `body`::`Any`; _mediaType=nothing) -> `InventoryCount`, `OpenAPI.Clients.ApiResponse` <br/>
> `update_inventory_count`(_api::`InventoryCountApi`, response_stream::`Channel`, `inventory_count_id`::`String`, `body`::`Any`; _mediaType=nothing) -> `Channel`{ `InventoryCount` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`InventoryCountApi`** | API context | 
**`inventory_count_id`** | **`String`** |  |
**`body`** | **`Any`** |  |

### Return type

[**`InventoryCount`**](InventoryCount.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **update_inventory_count_status**
> `update_inventory_count_status`(_api::`InventoryCountApi`, `inventory_count_id`::`String`, `inventory_count_status_update`::`InventoryCountStatusUpdate`; _mediaType=nothing) -> `InventoryCount`, `OpenAPI.Clients.ApiResponse` <br/>
> `update_inventory_count_status`(_api::`InventoryCountApi`, response_stream::`Channel`, `inventory_count_id`::`String`, `inventory_count_status_update`::`InventoryCountStatusUpdate`; _mediaType=nothing) -> `Channel`{ `InventoryCount` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`InventoryCountApi`** | API context | 
**`inventory_count_id`** | **`String`** |  |
**`inventory_count_status_update`** | [**`InventoryCountStatusUpdate`**](InventoryCountStatusUpdate.md) |  |

### Return type

[**`InventoryCount`**](InventoryCount.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

