# UstvaApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**jahresust_api**](UstvaApi.md#jahresust_api) | **GET** /api/v1/bookkeeping/jahresust | 
[**ustva_api**](UstvaApi.md#ustva_api) | **GET** /api/v1/bookkeeping/ustva | 


# **jahresust_api**
> `jahresust_api`(_api::`UstvaApi`, `year`::`Int64`; _mediaType=nothing) -> `JahresUstErgebnis`, `OpenAPI.Clients.ApiResponse` <br/>
> `jahresust_api`(_api::`UstvaApi`, response_stream::`Channel`, `year`::`Int64`; _mediaType=nothing) -> `Channel`{ `JahresUstErgebnis` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`UstvaApi`** | API context | 
**`year`** | **`Int64`** |  |

### Return type

[**`JahresUstErgebnis`**](JahresUstErgebnis.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **ustva_api**
> `ustva_api`(_api::`UstvaApi`, `zeitraum`::`String`; _mediaType=nothing) -> `UstvaErgebnis`, `OpenAPI.Clients.ApiResponse` <br/>
> `ustva_api`(_api::`UstvaApi`, response_stream::`Channel`, `zeitraum`::`String`; _mediaType=nothing) -> `Channel`{ `UstvaErgebnis` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`UstvaApi`** | API context | 
**`zeitraum`** | **`String`** |  |

### Return type

[**`UstvaErgebnis`**](UstvaErgebnis.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

