# ZugferdApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**generate_zugferd_api**](ZugferdApi.md#generate_zugferd_api) | **GET** /api/v1/invoices/{id}/zugferd | 


# **generate_zugferd_api**
> `generate_zugferd_api`(_api::`ZugferdApi`, `id`::`String`; `supplier_name`=nothing, `supplier_street`=nothing, `supplier_city`=nothing, `supplier_zip`=nothing, `supplier_country`=nothing, `supplier_vat_id`=nothing, _mediaType=nothing) -> `Nothing`, `OpenAPI.Clients.ApiResponse` <br/>
> `generate_zugferd_api`(_api::`ZugferdApi`, response_stream::`Channel`, `id`::`String`; `supplier_name`=nothing, `supplier_street`=nothing, `supplier_city`=nothing, `supplier_zip`=nothing, `supplier_country`=nothing, `supplier_vat_id`=nothing, _mediaType=nothing) -> `Channel`{ `Nothing` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ZugferdApi`** | API context | 
**`id`** | **`String`** |  |

### Optional Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **`supplier_name`** | **`String`** |  | [default to nothing]
 **`supplier_street`** | **`String`** |  | [default to nothing]
 **`supplier_city`** | **`String`** |  | [default to nothing]
 **`supplier_zip`** | **`String`** |  | [default to nothing]
 **`supplier_country`** | **`String`** |  | [default to nothing]
 **`supplier_vat_id`** | **`String`** |  | [default to nothing]

### Return type

`Nothing`

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/pdf

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

