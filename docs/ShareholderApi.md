# ShareholderApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_shareholder**](ShareholderApi.md#create_shareholder) | **POST** /api/v1/shareholders | 
[**delete_shareholder**](ShareholderApi.md#delete_shareholder) | **DELETE** /api/v1/shareholders/{id} | 
[**get_shareholder**](ShareholderApi.md#get_shareholder) | **GET** /api/v1/shareholders/{id} | 
[**get_shareholders**](ShareholderApi.md#get_shareholders) | **GET** /api/v1/shareholders/ | 
[**update_shareholder**](ShareholderApi.md#update_shareholder) | **PUT** /api/v1/shareholders/{id} | 


# **create_shareholder**
> `create_shareholder`(_api::`ShareholderApi`, `shareholder_create`::`ShareholderCreate`; _mediaType=nothing) -> `Shareholder`, `OpenAPI.Clients.ApiResponse` <br/>
> `create_shareholder`(_api::`ShareholderApi`, response_stream::`Channel`, `shareholder_create`::`ShareholderCreate`; _mediaType=nothing) -> `Channel`{ `Shareholder` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ShareholderApi`** | API context | 
**`shareholder_create`** | [**`ShareholderCreate`**](ShareholderCreate.md) |  |

### Return type

[**`Shareholder`**](Shareholder.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **delete_shareholder**
> `delete_shareholder`(_api::`ShareholderApi`, `id`::`String`; _mediaType=nothing) -> `Nothing`, `OpenAPI.Clients.ApiResponse` <br/>
> `delete_shareholder`(_api::`ShareholderApi`, response_stream::`Channel`, `id`::`String`; _mediaType=nothing) -> `Channel`{ `Nothing` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ShareholderApi`** | API context | 
**`id`** | **`String`** |  |

### Return type

`Nothing`

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **get_shareholder**
> `get_shareholder`(_api::`ShareholderApi`, `id`::`String`; _mediaType=nothing) -> `Shareholder`, `OpenAPI.Clients.ApiResponse` <br/>
> `get_shareholder`(_api::`ShareholderApi`, response_stream::`Channel`, `id`::`String`; _mediaType=nothing) -> `Channel`{ `Shareholder` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ShareholderApi`** | API context | 
**`id`** | **`String`** |  |

### Return type

[**`Shareholder`**](Shareholder.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **get_shareholders**
> `get_shareholders`(_api::`ShareholderApi`; `page`=nothing, `page_size`=nothing, `search`=nothing, `include_deleted`=nothing, _mediaType=nothing) -> `Vector{Shareholder}`, `OpenAPI.Clients.ApiResponse` <br/>
> `get_shareholders`(_api::`ShareholderApi`, response_stream::`Channel`; `page`=nothing, `page_size`=nothing, `search`=nothing, `include_deleted`=nothing, _mediaType=nothing) -> `Channel`{ `Vector{Shareholder}` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ShareholderApi`** | API context | 

### Optional Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **`page`** | **`Int64`** |  | [default to nothing]
 **`page_size`** | **`Int64`** |  | [default to nothing]
 **`search`** | **`String`** |  | [default to nothing]
 **`include_deleted`** | **`Bool`** | Soft-delete entities: set true to include rows with &#x60;deleted_at&#x60; set. | [default to nothing]

### Return type

[**`Vector{Shareholder}`**](Shareholder.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **update_shareholder**
> `update_shareholder`(_api::`ShareholderApi`, `id`::`String`, `shareholder_update`::`ShareholderUpdate`; _mediaType=nothing) -> `Shareholder`, `OpenAPI.Clients.ApiResponse` <br/>
> `update_shareholder`(_api::`ShareholderApi`, response_stream::`Channel`, `id`::`String`, `shareholder_update`::`ShareholderUpdate`; _mediaType=nothing) -> `Channel`{ `Shareholder` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ShareholderApi`** | API context | 
**`id`** | **`String`** |  |
**`shareholder_update`** | [**`ShareholderUpdate`**](ShareholderUpdate.md) |  |

### Return type

[**`Shareholder`**](Shareholder.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

