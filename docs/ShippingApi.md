# ShippingApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_credentials_api**](ShippingApi.md#get_credentials_api) | **GET** /api/v1/shipping/credentials | 
[**get_rates_api**](ShippingApi.md#get_rates_api) | **POST** /api/v1/shipping/rates | 
[**list_providers_api**](ShippingApi.md#list_providers_api) | **GET** /api/v1/shipping/providers | 
[**save_credentials_api**](ShippingApi.md#save_credentials_api) | **PUT** /api/v1/shipping/credentials | 


# **get_credentials_api**
> `get_credentials_api`(_api::`ShippingApi`; _mediaType=nothing) -> `ShippingCredentials`, `OpenAPI.Clients.ApiResponse` <br/>
> `get_credentials_api`(_api::`ShippingApi`, response_stream::`Channel`; _mediaType=nothing) -> `Channel`{ `ShippingCredentials` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters
This endpoint does not need any parameter.

### Return type

[**`ShippingCredentials`**](ShippingCredentials.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **get_rates_api**
> `get_rates_api`(_api::`ShippingApi`, `rate_request`::`RateRequest`; _mediaType=nothing) -> `RateResponse`, `OpenAPI.Clients.ApiResponse` <br/>
> `get_rates_api`(_api::`ShippingApi`, response_stream::`Channel`, `rate_request`::`RateRequest`; _mediaType=nothing) -> `Channel`{ `RateResponse` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ShippingApi`** | API context | 
**`rate_request`** | [**`RateRequest`**](RateRequest.md) |  |

### Return type

[**`RateResponse`**](RateResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **list_providers_api**
> `list_providers_api`(_api::`ShippingApi`; _mediaType=nothing) -> `Vector{ProviderInfo}`, `OpenAPI.Clients.ApiResponse` <br/>
> `list_providers_api`(_api::`ShippingApi`, response_stream::`Channel`; _mediaType=nothing) -> `Channel`{ `Vector{ProviderInfo}` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters
This endpoint does not need any parameter.

### Return type

[**`Vector{ProviderInfo}`**](ProviderInfo.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **save_credentials_api**
> `save_credentials_api`(_api::`ShippingApi`, `shipping_credentials`::`ShippingCredentials`; _mediaType=nothing) -> `ShippingCredentials`, `OpenAPI.Clients.ApiResponse` <br/>
> `save_credentials_api`(_api::`ShippingApi`, response_stream::`Channel`, `shipping_credentials`::`ShippingCredentials`; _mediaType=nothing) -> `Channel`{ `ShippingCredentials` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ShippingApi`** | API context | 
**`shipping_credentials`** | [**`ShippingCredentials`**](ShippingCredentials.md) |  |

### Return type

[**`ShippingCredentials`**](ShippingCredentials.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

