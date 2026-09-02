# KonzernApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**konzern_export_api**](KonzernApi.md#konzern_export_api) | **GET** /api/v1/bookkeeping/konzern/status/export | 
[**konzern_status_api**](KonzernApi.md#konzern_status_api) | **GET** /api/v1/bookkeeping/konzern/status | 


# **konzern_export_api**
> `konzern_export_api`(_api::`KonzernApi`, `year`::`Int64`; _mediaType=nothing) -> `KonzernExportResponse`, `OpenAPI.Clients.ApiResponse` <br/>
> `konzern_export_api`(_api::`KonzernApi`, response_stream::`Channel`, `year`::`Int64`; _mediaType=nothing) -> `Channel`{ `KonzernExportResponse` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`KonzernApi`** | API context | 
**`year`** | **`Int64`** |  |

### Return type

[**`KonzernExportResponse`**](KonzernExportResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **konzern_status_api**
> `konzern_status_api`(_api::`KonzernApi`, `year`::`Int64`; _mediaType=nothing) -> `KonzernStatus`, `OpenAPI.Clients.ApiResponse` <br/>
> `konzern_status_api`(_api::`KonzernApi`, response_stream::`Channel`, `year`::`Int64`; _mediaType=nothing) -> `Channel`{ `KonzernStatus` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`KonzernApi`** | API context | 
**`year`** | **`Int64`** |  |

### Return type

[**`KonzernStatus`**](KonzernStatus.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

