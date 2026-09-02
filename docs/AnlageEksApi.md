# AnlageEksApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**eks_api**](AnlageEksApi.md#eks_api) | **GET** /api/v1/bookkeeping/eks | 


# **eks_api**
> `eks_api`(_api::`AnlageEksApi`, `year`::`Int64`; _mediaType=nothing) -> `EksErgebnis`, `OpenAPI.Clients.ApiResponse` <br/>
> `eks_api`(_api::`AnlageEksApi`, response_stream::`Channel`, `year`::`Int64`; _mediaType=nothing) -> `Channel`{ `EksErgebnis` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`AnlageEksApi`** | API context | 
**`year`** | **`Int64`** |  |

### Return type

[**`EksErgebnis`**](EksErgebnis.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

