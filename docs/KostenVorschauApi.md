# KostenVorschauApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**kosten_vorschau_api**](KostenVorschauApi.md#kosten_vorschau_api) | **GET** /api/v1/bookkeeping/kosten-vorschau | 


# **kosten_vorschau_api**
> `kosten_vorschau_api`(_api::`KostenVorschauApi`, `year`::`Int64`, `month`::`Int64`; _mediaType=nothing) -> `KostenVorschau`, `OpenAPI.Clients.ApiResponse` <br/>
> `kosten_vorschau_api`(_api::`KostenVorschauApi`, response_stream::`Channel`, `year`::`Int64`, `month`::`Int64`; _mediaType=nothing) -> `Channel`{ `KostenVorschau` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`KostenVorschauApi`** | API context | 
**`year`** | **`Int64`** |  |
**`month`** | **`Int64`** |  |

### Return type

[**`KostenVorschau`**](KostenVorschau.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

