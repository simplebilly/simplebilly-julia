# PaygapApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**paygap_auskunft_api**](PaygapApi.md#paygap_auskunft_api) | **GET** /api/v1/bookkeeping/paygap/auskunft/{employee_id} | 
[**paygap_export_api**](PaygapApi.md#paygap_export_api) | **GET** /api/v1/bookkeeping/paygap/export | 
[**paygap_report_api**](PaygapApi.md#paygap_report_api) | **GET** /api/v1/bookkeeping/paygap/report | 


# **paygap_auskunft_api**
> `paygap_auskunft_api`(_api::`PaygapApi`, `employee_id`::`String`; _mediaType=nothing) -> `PayGapInfoResponse`, `OpenAPI.Clients.ApiResponse` <br/>
> `paygap_auskunft_api`(_api::`PaygapApi`, response_stream::`Channel`, `employee_id`::`String`; _mediaType=nothing) -> `Channel`{ `PayGapInfoResponse` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`PaygapApi`** | API context | 
**`employee_id`** | **`String`** |  |

### Return type

[**`PayGapInfoResponse`**](PayGapInfoResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **paygap_export_api**
> `paygap_export_api`(_api::`PaygapApi`; _mediaType=nothing) -> `PayGapExportResponse`, `OpenAPI.Clients.ApiResponse` <br/>
> `paygap_export_api`(_api::`PaygapApi`, response_stream::`Channel`; _mediaType=nothing) -> `Channel`{ `PayGapExportResponse` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters
This endpoint does not need any parameter.

### Return type

[**`PayGapExportResponse`**](PayGapExportResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **paygap_report_api**
> `paygap_report_api`(_api::`PaygapApi`; _mediaType=nothing) -> `PayGapReport`, `OpenAPI.Clients.ApiResponse` <br/>
> `paygap_report_api`(_api::`PaygapApi`, response_stream::`Channel`; _mediaType=nothing) -> `Channel`{ `PayGapReport` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters
This endpoint does not need any parameter.

### Return type

[**`PayGapReport`**](PayGapReport.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

