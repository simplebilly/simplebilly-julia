# ReplenishmentApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**apply_replenishments**](ReplenishmentApi.md#apply_replenishments) | **POST** /api/v1/replenishments/apply | Create one draft stock transfer per (source → target) pair carrying all suggested product lines for that pair.
[**get_replenishments**](ReplenishmentApi.md#get_replenishments) | **GET** /api/v1/replenishments | 


# **apply_replenishments**
> `apply_replenishments`(_api::`ReplenishmentApi`; `target_warehouse_id`=nothing, `source_warehouse_id`=nothing, _mediaType=nothing) -> `Any`, `OpenAPI.Clients.ApiResponse` <br/>
> `apply_replenishments`(_api::`ReplenishmentApi`, response_stream::`Channel`; `target_warehouse_id`=nothing, `source_warehouse_id`=nothing, _mediaType=nothing) -> `Channel`{ `Any` }, `OpenAPI.Clients.ApiResponse`

Create one draft stock transfer per (source → target) pair carrying all suggested product lines for that pair.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ReplenishmentApi`** | API context | 

### Optional Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **`target_warehouse_id`** | **`String`** | Warehouse to be replenished. Defaults to the tenant&#39;s default warehouse. | [default to nothing]
 **`source_warehouse_id`** | **`String`** | Restrict source warehouses to this id. | [default to nothing]

### Return type

**`Any`**

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **get_replenishments**
> `get_replenishments`(_api::`ReplenishmentApi`; `target_warehouse_id`=nothing, `source_warehouse_id`=nothing, _mediaType=nothing) -> `ReplenishmentResponse`, `OpenAPI.Clients.ApiResponse` <br/>
> `get_replenishments`(_api::`ReplenishmentApi`, response_stream::`Channel`; `target_warehouse_id`=nothing, `source_warehouse_id`=nothing, _mediaType=nothing) -> `Channel`{ `ReplenishmentResponse` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ReplenishmentApi`** | API context | 

### Optional Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **`target_warehouse_id`** | **`String`** | Warehouse to be replenished. Defaults to the tenant&#39;s default warehouse. | [default to nothing]
 **`source_warehouse_id`** | **`String`** | Restrict source warehouses to this id. | [default to nothing]

### Return type

[**`ReplenishmentResponse`**](ReplenishmentResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

