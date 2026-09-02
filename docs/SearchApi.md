# SearchApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**global_search**](SearchApi.md#global_search) | **GET** /api/v1/search | GET /api/v1/search?q&#x3D;...
[**my_permissions**](SearchApi.md#my_permissions) | **GET** /api/v1/me/permissions | GET /api/v1/me/permissions — resolved permissions from the auth token, used by the frontend to show/hide admin navigation.


# **global_search**
> `global_search`(_api::`SearchApi`, `q`::`String`; _mediaType=nothing) -> `Any`, `OpenAPI.Clients.ApiResponse` <br/>
> `global_search`(_api::`SearchApi`, response_stream::`Channel`, `q`::`String`; _mediaType=nothing) -> `Channel`{ `Any` }, `OpenAPI.Clients.ApiResponse`

GET /api/v1/search?q=...

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`SearchApi`** | API context | 
**`q`** | **`String`** | Search text (min 2 chars) |

### Return type

**`Any`**

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **my_permissions**
> `my_permissions`(_api::`SearchApi`; _mediaType=nothing) -> `Any`, `OpenAPI.Clients.ApiResponse` <br/>
> `my_permissions`(_api::`SearchApi`, response_stream::`Channel`; _mediaType=nothing) -> `Channel`{ `Any` }, `OpenAPI.Clients.ApiResponse`

GET /api/v1/me/permissions — resolved permissions from the auth token, used by the frontend to show/hide admin navigation.

### Required Parameters
This endpoint does not need any parameter.

### Return type

**`Any`**

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

