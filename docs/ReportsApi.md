# ReportsApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**bilanz_report_api**](ReportsApi.md#bilanz_report_api) | **GET** /api/v1/bookkeeping/reports/bilanz | Bilanz (Balance Sheet)
[**guv_report_api**](ReportsApi.md#guv_report_api) | **GET** /api/v1/bookkeeping/reports/guv | Gewinn- und Verlustrechnung (P&amp;L statement)
[**kontenansicht_report_api**](ReportsApi.md#kontenansicht_report_api) | **GET** /api/v1/bookkeeping/reports/kontenansicht | Kontenansicht (Account Overview)
[**umsatzsteuer_report_api**](ReportsApi.md#umsatzsteuer_report_api) | **GET** /api/v1/bookkeeping/reports/umsatzsteuer | Umsatzsteuer-Voranmeldung (VAT report)


# **bilanz_report_api**
> `bilanz_report_api`(_api::`ReportsApi`; `year`=nothing, `month`=nothing, `date_from`=nothing, `date_to`=nothing, `page`=nothing, `page_size`=nothing, _mediaType=nothing) -> `BilanzReport`, `OpenAPI.Clients.ApiResponse` <br/>
> `bilanz_report_api`(_api::`ReportsApi`, response_stream::`Channel`; `year`=nothing, `month`=nothing, `date_from`=nothing, `date_to`=nothing, `page`=nothing, `page_size`=nothing, _mediaType=nothing) -> `Channel`{ `BilanzReport` }, `OpenAPI.Clients.ApiResponse`

Bilanz (Balance Sheet)

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ReportsApi`** | API context | 

### Optional Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **`year`** | **`Int64`** |  | [default to nothing]
 **`month`** | **`Int64`** |  | [default to nothing]
 **`date_from`** | **`String`** |  | [default to nothing]
 **`date_to`** | **`String`** |  | [default to nothing]
 **`page`** | **`Int64`** |  | [default to nothing]
 **`page_size`** | **`Int64`** |  | [default to nothing]

### Return type

[**`BilanzReport`**](BilanzReport.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **guv_report_api**
> `guv_report_api`(_api::`ReportsApi`; `year`=nothing, `month`=nothing, `date_from`=nothing, `date_to`=nothing, `page`=nothing, `page_size`=nothing, _mediaType=nothing) -> `GuVReport`, `OpenAPI.Clients.ApiResponse` <br/>
> `guv_report_api`(_api::`ReportsApi`, response_stream::`Channel`; `year`=nothing, `month`=nothing, `date_from`=nothing, `date_to`=nothing, `page`=nothing, `page_size`=nothing, _mediaType=nothing) -> `Channel`{ `GuVReport` }, `OpenAPI.Clients.ApiResponse`

Gewinn- und Verlustrechnung (P&L statement)

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ReportsApi`** | API context | 

### Optional Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **`year`** | **`Int64`** |  | [default to nothing]
 **`month`** | **`Int64`** |  | [default to nothing]
 **`date_from`** | **`String`** |  | [default to nothing]
 **`date_to`** | **`String`** |  | [default to nothing]
 **`page`** | **`Int64`** |  | [default to nothing]
 **`page_size`** | **`Int64`** |  | [default to nothing]

### Return type

[**`GuVReport`**](GuVReport.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **kontenansicht_report_api**
> `kontenansicht_report_api`(_api::`ReportsApi`; `year`=nothing, `month`=nothing, `date_from`=nothing, `date_to`=nothing, `page`=nothing, `page_size`=nothing, _mediaType=nothing) -> `KontoReport`, `OpenAPI.Clients.ApiResponse` <br/>
> `kontenansicht_report_api`(_api::`ReportsApi`, response_stream::`Channel`; `year`=nothing, `month`=nothing, `date_from`=nothing, `date_to`=nothing, `page`=nothing, `page_size`=nothing, _mediaType=nothing) -> `Channel`{ `KontoReport` }, `OpenAPI.Clients.ApiResponse`

Kontenansicht (Account Overview)

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ReportsApi`** | API context | 

### Optional Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **`year`** | **`Int64`** |  | [default to nothing]
 **`month`** | **`Int64`** |  | [default to nothing]
 **`date_from`** | **`String`** |  | [default to nothing]
 **`date_to`** | **`String`** |  | [default to nothing]
 **`page`** | **`Int64`** |  | [default to nothing]
 **`page_size`** | **`Int64`** |  | [default to nothing]

### Return type

[**`KontoReport`**](KontoReport.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **umsatzsteuer_report_api**
> `umsatzsteuer_report_api`(_api::`ReportsApi`; `year`=nothing, `month`=nothing, `date_from`=nothing, `date_to`=nothing, `page`=nothing, `page_size`=nothing, _mediaType=nothing) -> `UmsatzsteuerReport`, `OpenAPI.Clients.ApiResponse` <br/>
> `umsatzsteuer_report_api`(_api::`ReportsApi`, response_stream::`Channel`; `year`=nothing, `month`=nothing, `date_from`=nothing, `date_to`=nothing, `page`=nothing, `page_size`=nothing, _mediaType=nothing) -> `Channel`{ `UmsatzsteuerReport` }, `OpenAPI.Clients.ApiResponse`

Umsatzsteuer-Voranmeldung (VAT report)

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ReportsApi`** | API context | 

### Optional Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **`year`** | **`Int64`** |  | [default to nothing]
 **`month`** | **`Int64`** |  | [default to nothing]
 **`date_from`** | **`String`** |  | [default to nothing]
 **`date_to`** | **`String`** |  | [default to nothing]
 **`page`** | **`Int64`** |  | [default to nothing]
 **`page_size`** | **`Int64`** |  | [default to nothing]

### Return type

[**`UmsatzsteuerReport`**](UmsatzsteuerReport.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

