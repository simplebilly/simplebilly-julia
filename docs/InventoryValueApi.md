# InventoryValueApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_inventory_value_api**](InventoryValueApi.md#get_inventory_value_api) | **GET** /api/v1/bookkeeping/inventory-value | 
[**record_inventory_value_api**](InventoryValueApi.md#record_inventory_value_api) | **POST** /api/v1/bookkeeping/inventory-value/record | 


# **get_inventory_value_api**
> `get_inventory_value_api`(_api::`InventoryValueApi`; _mediaType=nothing) -> `CurrentInventoryValue`, `OpenAPI.Clients.ApiResponse` <br/>
> `get_inventory_value_api`(_api::`InventoryValueApi`, response_stream::`Channel`; _mediaType=nothing) -> `Channel`{ `CurrentInventoryValue` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters
This endpoint does not need any parameter.

### Return type

[**`CurrentInventoryValue`**](CurrentInventoryValue.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **record_inventory_value_api**
> `record_inventory_value_api`(_api::`InventoryValueApi`; _mediaType=nothing) -> `InventoryValuePoint`, `OpenAPI.Clients.ApiResponse` <br/>
> `record_inventory_value_api`(_api::`InventoryValueApi`, response_stream::`Channel`; _mediaType=nothing) -> `Channel`{ `InventoryValuePoint` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters
This endpoint does not need any parameter.

### Return type

[**`InventoryValuePoint`**](InventoryValuePoint.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

