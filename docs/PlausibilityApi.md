# PlausibilityApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**plausibility_check_api**](PlausibilityApi.md#plausibility_check_api) | **GET** /api/v1/bookkeeping/plausibility | 


# **plausibility_check_api**
> `plausibility_check_api`(_api::`PlausibilityApi`; `date_from`=nothing, `date_to`=nothing, _mediaType=nothing) -> `PlausibilityReport`, `OpenAPI.Clients.ApiResponse` <br/>
> `plausibility_check_api`(_api::`PlausibilityApi`, response_stream::`Channel`; `date_from`=nothing, `date_to`=nothing, _mediaType=nothing) -> `Channel`{ `PlausibilityReport` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`PlausibilityApi`** | API context | 

### Optional Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **`date_from`** | **`String`** |  | [default to nothing]
 **`date_to`** | **`String`** |  | [default to nothing]

### Return type

[**`PlausibilityReport`**](PlausibilityReport.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

