# GobdExportApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**buchhalter_csv_api**](GobdExportApi.md#buchhalter_csv_api) | **GET** /api/v1/bookkeeping/buchhalter-csv | 
[**gobd_export_api**](GobdExportApi.md#gobd_export_api) | **GET** /api/v1/bookkeeping/gobd | GoBD/GDPdU export. Default: ZIP archive (&#x60;index.xml&#x60; + CSV tables, IDEA format). &#x60;?format&#x3D;csv&#x60; returns the legacy single-journal CSV as JSON.


# **buchhalter_csv_api**
> `buchhalter_csv_api`(_api::`GobdExportApi`, `date_from`::`String`, `date_to`::`String`; _mediaType=nothing) -> `GoBDExportResponse`, `OpenAPI.Clients.ApiResponse` <br/>
> `buchhalter_csv_api`(_api::`GobdExportApi`, response_stream::`Channel`, `date_from`::`String`, `date_to`::`String`; _mediaType=nothing) -> `Channel`{ `GoBDExportResponse` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`GobdExportApi`** | API context | 
**`date_from`** | **`String`** |  |
**`date_to`** | **`String`** |  |

### Return type

[**`GoBDExportResponse`**](GoBDExportResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **gobd_export_api**
> `gobd_export_api`(_api::`GobdExportApi`, `year`::`Int64`; `format`=nothing, _mediaType=nothing) -> `Nothing`, `OpenAPI.Clients.ApiResponse` <br/>
> `gobd_export_api`(_api::`GobdExportApi`, response_stream::`Channel`, `year`::`Int64`; `format`=nothing, _mediaType=nothing) -> `Channel`{ `Nothing` }, `OpenAPI.Clients.ApiResponse`

GoBD/GDPdU export. Default: ZIP archive (`index.xml` + CSV tables, IDEA format). `?format=csv` returns the legacy single-journal CSV as JSON.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`GobdExportApi`** | API context | 
**`year`** | **`Int64`** |  |

### Optional Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **`format`** | **`String`** | Export format: &#x60;zip&#x60; (default, full GDPdU/IDEA export) or &#x60;csv&#x60; (legacy single-journal CSV as JSON). | [default to nothing]

### Return type

`Nothing`

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/zip, application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

