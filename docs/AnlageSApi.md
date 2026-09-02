# AnlageSApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**anlage_s_api**](AnlageSApi.md#anlage_s_api) | **GET** /api/v1/bookkeeping/anlage-s | 


# **anlage_s_api**
> `anlage_s_api`(_api::`AnlageSApi`, `year`::`Int64`; _mediaType=nothing) -> `AnlageSErgebnis`, `OpenAPI.Clients.ApiResponse` <br/>
> `anlage_s_api`(_api::`AnlageSApi`, response_stream::`Channel`, `year`::`Int64`; _mediaType=nothing) -> `Channel`{ `AnlageSErgebnis` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`AnlageSApi`** | API context | 
**`year`** | **`Int64`** |  |

### Return type

[**`AnlageSErgebnis`**](AnlageSErgebnis.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

