# AnlageGApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**anlage_g_api**](AnlageGApi.md#anlage_g_api) | **GET** /api/v1/bookkeeping/anlage-g | 


# **anlage_g_api**
> `anlage_g_api`(_api::`AnlageGApi`, `year`::`Int64`; _mediaType=nothing) -> `AnlageGErgebnis`, `OpenAPI.Clients.ApiResponse` <br/>
> `anlage_g_api`(_api::`AnlageGApi`, response_stream::`Channel`, `year`::`Int64`; _mediaType=nothing) -> `Channel`{ `AnlageGErgebnis` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`AnlageGApi`** | API context | 
**`year`** | **`Int64`** |  |

### Return type

[**`AnlageGErgebnis`**](AnlageGErgebnis.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

