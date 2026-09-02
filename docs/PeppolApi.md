# PeppolApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**peppol_api**](PeppolApi.md#peppol_api) | **GET** /api/v1/invoices/{id}/peppol | 


# **peppol_api**
> `peppol_api`(_api::`PeppolApi`, `id`::`String`; _mediaType=nothing) -> `PeppolResponse`, `OpenAPI.Clients.ApiResponse` <br/>
> `peppol_api`(_api::`PeppolApi`, response_stream::`Channel`, `id`::`String`; _mediaType=nothing) -> `Channel`{ `PeppolResponse` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`PeppolApi`** | API context | 
**`id`** | **`String`** |  |

### Return type

[**`PeppolResponse`**](PeppolResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

