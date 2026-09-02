# KstApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**kst_api**](KstApi.md#kst_api) | **GET** /api/v1/bookkeeping/kst | 


# **kst_api**
> `kst_api`(_api::`KstApi`, `year`::`Int64`; `gewinn`=nothing, _mediaType=nothing) -> `KstErgebnis`, `OpenAPI.Clients.ApiResponse` <br/>
> `kst_api`(_api::`KstApi`, response_stream::`Channel`, `year`::`Int64`; `gewinn`=nothing, _mediaType=nothing) -> `Channel`{ `KstErgebnis` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`KstApi`** | API context | 
**`year`** | **`Int64`** |  |

### Optional Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **`gewinn`** | **`String`** |  | [default to nothing]

### Return type

[**`KstErgebnis`**](KstErgebnis.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

