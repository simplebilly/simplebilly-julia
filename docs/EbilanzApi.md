# EbilanzApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ebilanz_report_api**](EbilanzApi.md#ebilanz_report_api) | **GET** /api/v1/bookkeeping/ebilanz | 
[**ebilanz_xbrl_export_api**](EbilanzApi.md#ebilanz_xbrl_export_api) | **GET** /api/v1/bookkeeping/ebilanz/xbrl | 


# **ebilanz_report_api**
> `ebilanz_report_api`(_api::`EbilanzApi`; `year`=nothing, `date_from`=nothing, `date_to`=nothing, _mediaType=nothing) -> `EBilanzReport`, `OpenAPI.Clients.ApiResponse` <br/>
> `ebilanz_report_api`(_api::`EbilanzApi`, response_stream::`Channel`; `year`=nothing, `date_from`=nothing, `date_to`=nothing, _mediaType=nothing) -> `Channel`{ `EBilanzReport` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`EbilanzApi`** | API context | 

### Optional Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **`year`** | **`Int64`** |  | [default to nothing]
 **`date_from`** | **`String`** |  | [default to nothing]
 **`date_to`** | **`String`** |  | [default to nothing]

### Return type

[**`EBilanzReport`**](EBilanzReport.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **ebilanz_xbrl_export_api**
> `ebilanz_xbrl_export_api`(_api::`EbilanzApi`; `year`=nothing, `date_from`=nothing, `date_to`=nothing, _mediaType=nothing) -> `Nothing`, `OpenAPI.Clients.ApiResponse` <br/>
> `ebilanz_xbrl_export_api`(_api::`EbilanzApi`, response_stream::`Channel`; `year`=nothing, `date_from`=nothing, `date_to`=nothing, _mediaType=nothing) -> `Channel`{ `Nothing` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`EbilanzApi`** | API context | 

### Optional Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **`year`** | **`Int64`** |  | [default to nothing]
 **`date_from`** | **`String`** |  | [default to nothing]
 **`date_to`** | **`String`** |  | [default to nothing]

### Return type

`Nothing`

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/xml

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

