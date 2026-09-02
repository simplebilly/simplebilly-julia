# StilleApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**stille_export_api**](StilleApi.md#stille_export_api) | **GET** /api/v1/bookkeeping/stille/export | 
[**stille_report_api**](StilleApi.md#stille_report_api) | **GET** /api/v1/bookkeeping/stille/report | 


# **stille_export_api**
> `stille_export_api`(_api::`StilleApi`, `year`::`Int64`; _mediaType=nothing) -> `StilleExportResponse`, `OpenAPI.Clients.ApiResponse` <br/>
> `stille_export_api`(_api::`StilleApi`, response_stream::`Channel`, `year`::`Int64`; _mediaType=nothing) -> `Channel`{ `StilleExportResponse` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`StilleApi`** | API context | 
**`year`** | **`Int64`** |  |

### Return type

[**`StilleExportResponse`**](StilleExportResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **stille_report_api**
> `stille_report_api`(_api::`StilleApi`, `year`::`Int64`; _mediaType=nothing) -> `StilleReport`, `OpenAPI.Clients.ApiResponse` <br/>
> `stille_report_api`(_api::`StilleApi`, response_stream::`Channel`, `year`::`Int64`; _mediaType=nothing) -> `Channel`{ `StilleReport` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`StilleApi`** | API context | 
**`year`** | **`Int64`** |  |

### Return type

[**`StilleReport`**](StilleReport.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

