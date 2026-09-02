# GenerateXrechnungApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**generate_xrechnung_api**](GenerateXrechnungApi.md#generate_xrechnung_api) | **GET** /api/v1/invoices/{id}/xrechnung | 


# **generate_xrechnung_api**
> `generate_xrechnung_api`(_api::`GenerateXrechnungApi`, `id`::`String`; `supplier_name`=nothing, `supplier_street`=nothing, `supplier_city`=nothing, `supplier_zip`=nothing, `supplier_country`=nothing, `supplier_vat_id`=nothing, _mediaType=nothing) -> `XRechnungResponse`, `OpenAPI.Clients.ApiResponse` <br/>
> `generate_xrechnung_api`(_api::`GenerateXrechnungApi`, response_stream::`Channel`, `id`::`String`; `supplier_name`=nothing, `supplier_street`=nothing, `supplier_city`=nothing, `supplier_zip`=nothing, `supplier_country`=nothing, `supplier_vat_id`=nothing, _mediaType=nothing) -> `Channel`{ `XRechnungResponse` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`GenerateXrechnungApi`** | API context | 
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

[**`XRechnungResponse`**](XRechnungResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

