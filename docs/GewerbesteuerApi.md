# GewerbesteuerApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**gewerbesteuer_api**](GewerbesteuerApi.md#gewerbesteuer_api) | **GET** /api/v1/bookkeeping/gewerbesteuer | 


# **gewerbesteuer_api**
> `gewerbesteuer_api`(_api::`GewerbesteuerApi`, `year`::`Int64`; `hebesatz`=nothing, `gewerbeertrag`=nothing, `country`=nothing, `gemeindeschluessel`=nothing, _mediaType=nothing) -> `GewerbesteuerErgebnis`, `OpenAPI.Clients.ApiResponse` <br/>
> `gewerbesteuer_api`(_api::`GewerbesteuerApi`, response_stream::`Channel`, `year`::`Int64`; `hebesatz`=nothing, `gewerbeertrag`=nothing, `country`=nothing, `gemeindeschluessel`=nothing, _mediaType=nothing) -> `Channel`{ `GewerbesteuerErgebnis` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`GewerbesteuerApi`** | API context | 
**`year`** | **`Int64`** |  |

### Optional Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **`hebesatz`** | **`String`** |  | [default to nothing]
 **`gewerbeertrag`** | **`String`** |  | [default to nothing]
 **`country`** | **`String`** |  | [default to nothing]
 **`gemeindeschluessel`** | **`String`** |  | [default to nothing]

### Return type

[**`GewerbesteuerErgebnis`**](GewerbesteuerErgebnis.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

