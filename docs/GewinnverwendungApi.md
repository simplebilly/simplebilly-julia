# GewinnverwendungApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**gewinnverwendung_api**](GewinnverwendungApi.md#gewinnverwendung_api) | **GET** /api/v1/bookkeeping/gewinnverwendung | 
[**gewinnverwendung_export_api**](GewinnverwendungApi.md#gewinnverwendung_export_api) | **GET** /api/v1/bookkeeping/gewinnverwendung/export | 


# **gewinnverwendung_api**
> `gewinnverwendung_api`(_api::`GewinnverwendungApi`, `year`::`Int64`; _mediaType=nothing) -> `GewinnverwendungsReport`, `OpenAPI.Clients.ApiResponse` <br/>
> `gewinnverwendung_api`(_api::`GewinnverwendungApi`, response_stream::`Channel`, `year`::`Int64`; _mediaType=nothing) -> `Channel`{ `GewinnverwendungsReport` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`GewinnverwendungApi`** | API context | 
**`year`** | **`Int64`** |  |

### Return type

[**`GewinnverwendungsReport`**](GewinnverwendungsReport.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **gewinnverwendung_export_api**
> `gewinnverwendung_export_api`(_api::`GewinnverwendungApi`, `year`::`Int64`; _mediaType=nothing) -> `GewinnverwendungsExportResponse`, `OpenAPI.Clients.ApiResponse` <br/>
> `gewinnverwendung_export_api`(_api::`GewinnverwendungApi`, response_stream::`Channel`, `year`::`Int64`; _mediaType=nothing) -> `Channel`{ `GewinnverwendungsExportResponse` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`GewinnverwendungApi`** | API context | 
**`year`** | **`Int64`** |  |

### Return type

[**`GewinnverwendungsExportResponse`**](GewinnverwendungsExportResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

