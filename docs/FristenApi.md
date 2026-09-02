# FristenApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**fristen_api**](FristenApi.md#fristen_api) | **GET** /api/v1/bookkeeping/fristen | 


# **fristen_api**
> `fristen_api`(_api::`FristenApi`; `bundesland`=nothing, `voranmeldungsrhythmus`=nothing, `dauerfristverlaengerung`=nothing, `est_aktiv`=nothing, `gewst_aktiv`=nothing, `monate`=nothing, _mediaType=nothing) -> `FristenErgebnis`, `OpenAPI.Clients.ApiResponse` <br/>
> `fristen_api`(_api::`FristenApi`, response_stream::`Channel`; `bundesland`=nothing, `voranmeldungsrhythmus`=nothing, `dauerfristverlaengerung`=nothing, `est_aktiv`=nothing, `gewst_aktiv`=nothing, `monate`=nothing, _mediaType=nothing) -> `Channel`{ `FristenErgebnis` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`FristenApi`** | API context | 

### Optional Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **`bundesland`** | **`String`** |  | [default to nothing]
 **`voranmeldungsrhythmus`** | **`String`** |  | [default to nothing]
 **`dauerfristverlaengerung`** | **`Bool`** |  | [default to nothing]
 **`est_aktiv`** | **`Bool`** |  | [default to nothing]
 **`gewst_aktiv`** | **`Bool`** |  | [default to nothing]
 **`monate`** | **`Int64`** |  | [default to nothing]

### Return type

[**`FristenErgebnis`**](FristenErgebnis.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

