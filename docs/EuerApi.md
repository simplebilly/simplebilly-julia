# EuerApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**euer_api**](EuerApi.md#euer_api) | **GET** /api/v1/bookkeeping/euer | 
[**euer_kategorien_api**](EuerApi.md#euer_kategorien_api) | **GET** /api/v1/bookkeeping/euer/kategorien | 


# **euer_api**
> `euer_api`(_api::`EuerApi`, `year`::`Int64`; _mediaType=nothing) -> `EuerErgebnis`, `OpenAPI.Clients.ApiResponse` <br/>
> `euer_api`(_api::`EuerApi`, response_stream::`Channel`, `year`::`Int64`; _mediaType=nothing) -> `Channel`{ `EuerErgebnis` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`EuerApi`** | API context | 
**`year`** | **`Int64`** |  |

### Return type

[**`EuerErgebnis`**](EuerErgebnis.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **euer_kategorien_api**
> `euer_kategorien_api`(_api::`EuerApi`, `year`::`Int64`; _mediaType=nothing) -> `EuerDetailErgebnis`, `OpenAPI.Clients.ApiResponse` <br/>
> `euer_kategorien_api`(_api::`EuerApi`, response_stream::`Channel`, `year`::`Int64`; _mediaType=nothing) -> `Channel`{ `EuerDetailErgebnis` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`EuerApi`** | API context | 
**`year`** | **`Int64`** |  |

### Return type

[**`EuerDetailErgebnis`**](EuerDetailErgebnis.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

