# DatevApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**datev_export_api**](DatevApi.md#datev_export_api) | **GET** /api/v1/bookkeeping/datev/export | Export bookkeeping data as DATEV CSV
[**datev_preview_api**](DatevApi.md#datev_preview_api) | **GET** /api/v1/bookkeeping/datev/preview | Exported_datev_bookings: returns formed bookings for review


# **datev_export_api**
> `datev_export_api`(_api::`DatevApi`; `account_schema`=nothing, `date_from`=nothing, `date_to`=nothing, `page`=nothing, `page_size`=nothing, _mediaType=nothing) -> `DatevExportResponse`, `OpenAPI.Clients.ApiResponse` <br/>
> `datev_export_api`(_api::`DatevApi`, response_stream::`Channel`; `account_schema`=nothing, `date_from`=nothing, `date_to`=nothing, `page`=nothing, `page_size`=nothing, _mediaType=nothing) -> `Channel`{ `DatevExportResponse` }, `OpenAPI.Clients.ApiResponse`

Export bookkeeping data as DATEV CSV

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`DatevApi`** | API context | 

### Optional Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **`account_schema`** | **`String`** |  | [default to nothing]
 **`date_from`** | **`String`** |  | [default to nothing]
 **`date_to`** | **`String`** |  | [default to nothing]
 **`page`** | **`Int64`** |  | [default to nothing]
 **`page_size`** | **`Int64`** |  | [default to nothing]

### Return type

[**`DatevExportResponse`**](DatevExportResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **datev_preview_api**
> `datev_preview_api`(_api::`DatevApi`; `account_schema`=nothing, `date_from`=nothing, `date_to`=nothing, `page`=nothing, `page_size`=nothing, _mediaType=nothing) -> `Vector{DatevBookingPreview}`, `OpenAPI.Clients.ApiResponse` <br/>
> `datev_preview_api`(_api::`DatevApi`, response_stream::`Channel`; `account_schema`=nothing, `date_from`=nothing, `date_to`=nothing, `page`=nothing, `page_size`=nothing, _mediaType=nothing) -> `Channel`{ `Vector{DatevBookingPreview}` }, `OpenAPI.Clients.ApiResponse`

Exported_datev_bookings: returns formed bookings for review

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`DatevApi`** | API context | 

### Optional Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **`account_schema`** | **`String`** |  | [default to nothing]
 **`date_from`** | **`String`** |  | [default to nothing]
 **`date_to`** | **`String`** |  | [default to nothing]
 **`page`** | **`Int64`** |  | [default to nothing]
 **`page_size`** | **`Int64`** |  | [default to nothing]

### Return type

[**`Vector{DatevBookingPreview}`**](DatevBookingPreview.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

