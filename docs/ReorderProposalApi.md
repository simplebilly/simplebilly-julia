# ReorderProposalApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**apply_reorder_proposal**](ReorderProposalApi.md#apply_reorder_proposal) | **POST** /api/v1/reorder-proposals/apply | Convert a reorder proposal into a draft purchase order.
[**get_reorder_proposal**](ReorderProposalApi.md#get_reorder_proposal) | **GET** /api/v1/reorder-proposals | 


# **apply_reorder_proposal**
> `apply_reorder_proposal`(_api::`ReorderProposalApi`; `configured_only`=nothing, `warehouse_id`=nothing, _mediaType=nothing) -> `Any`, `OpenAPI.Clients.ApiResponse` <br/>
> `apply_reorder_proposal`(_api::`ReorderProposalApi`, response_stream::`Channel`; `configured_only`=nothing, `warehouse_id`=nothing, _mediaType=nothing) -> `Channel`{ `Any` }, `OpenAPI.Clients.ApiResponse`

Convert a reorder proposal into a draft purchase order.

Returns the created purchase order id. Suggested line items are generated with the current reorder quantity per product.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ReorderProposalApi`** | API context | 

### Optional Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **`configured_only`** | **`Bool`** | Only include products with a reorder point configured (&#x60;min_stock&#x60;). | [default to nothing]
 **`warehouse_id`** | **`String`** | Limit to a single warehouse id. | [default to nothing]

### Return type

**`Any`**

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **get_reorder_proposal**
> `get_reorder_proposal`(_api::`ReorderProposalApi`; `configured_only`=nothing, `warehouse_id`=nothing, _mediaType=nothing) -> `ReorderProposalResponse`, `OpenAPI.Clients.ApiResponse` <br/>
> `get_reorder_proposal`(_api::`ReorderProposalApi`, response_stream::`Channel`; `configured_only`=nothing, `warehouse_id`=nothing, _mediaType=nothing) -> `Channel`{ `ReorderProposalResponse` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ReorderProposalApi`** | API context | 

### Optional Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **`configured_only`** | **`Bool`** | Only include products with a reorder point configured (&#x60;min_stock&#x60;). | [default to nothing]
 **`warehouse_id`** | **`String`** | Limit to a single warehouse id. | [default to nothing]

### Return type

[**`ReorderProposalResponse`**](ReorderProposalResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

