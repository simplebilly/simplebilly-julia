# ListOpenItemsApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**list_open_items_api**](ListOpenItemsApi.md#list_open_items_api) | **GET** /api/v1/bookkeeping/open-items | 


# **list_open_items_api**
> `list_open_items_api`(_api::`ListOpenItemsApi`; `reminder_level1_days`=nothing, `reminder_level2_days`=nothing, `reminder_level3_days`=nothing, `customer_id`=nothing, _mediaType=nothing) -> `Vector{OpenItem}`, `OpenAPI.Clients.ApiResponse` <br/>
> `list_open_items_api`(_api::`ListOpenItemsApi`, response_stream::`Channel`; `reminder_level1_days`=nothing, `reminder_level2_days`=nothing, `reminder_level3_days`=nothing, `customer_id`=nothing, _mediaType=nothing) -> `Channel`{ `Vector{OpenItem}` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ListOpenItemsApi`** | API context | 

### Optional Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **`reminder_level1_days`** | **`Int64`** |  | [default to nothing]
 **`reminder_level2_days`** | **`Int64`** |  | [default to nothing]
 **`reminder_level3_days`** | **`Int64`** |  | [default to nothing]
 **`customer_id`** | **`String`** |  | [default to nothing]

### Return type

[**`Vector{OpenItem}`**](OpenItem.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

