# SuitabilityApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**shipping_suitability_api**](SuitabilityApi.md#shipping_suitability_api) | **POST** /api/v1/shipping/suitability | 


# **shipping_suitability_api**
> `shipping_suitability_api`(_api::`SuitabilityApi`, `suitability_request`::`SuitabilityRequest`; _mediaType=nothing) -> `SuitabilityResult`, `OpenAPI.Clients.ApiResponse` <br/>
> `shipping_suitability_api`(_api::`SuitabilityApi`, response_stream::`Channel`, `suitability_request`::`SuitabilityRequest`; _mediaType=nothing) -> `Channel`{ `SuitabilityResult` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`SuitabilityApi`** | API context | 
**`suitability_request`** | [**`SuitabilityRequest`**](SuitabilityRequest.md) |  |

### Return type

[**`SuitabilityResult`**](SuitabilityResult.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

