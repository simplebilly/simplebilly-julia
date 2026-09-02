# BomApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_bom**](BomApi.md#create_bom) | **POST** /api/v1/boms | 
[**delete_bom**](BomApi.md#delete_bom) | **DELETE** /api/v1/boms/{bom_id} | 
[**get_bom**](BomApi.md#get_bom) | **GET** /api/v1/boms/{bom_id} | 
[**list_boms**](BomApi.md#list_boms) | **GET** /api/v1/boms/ | 
[**update_bom**](BomApi.md#update_bom) | **PUT** /api/v1/boms/{bom_id} | 


# **create_bom**
> `create_bom`(_api::`BomApi`, `bom_create`::`BomCreate`; _mediaType=nothing) -> `Bom`, `OpenAPI.Clients.ApiResponse` <br/>
> `create_bom`(_api::`BomApi`, response_stream::`Channel`, `bom_create`::`BomCreate`; _mediaType=nothing) -> `Channel`{ `Bom` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`BomApi`** | API context | 
**`bom_create`** | [**`BomCreate`**](BomCreate.md) |  |

### Return type

[**`Bom`**](Bom.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **delete_bom**
> `delete_bom`(_api::`BomApi`, `bom_id`::`String`; _mediaType=nothing) -> `Nothing`, `OpenAPI.Clients.ApiResponse` <br/>
> `delete_bom`(_api::`BomApi`, response_stream::`Channel`, `bom_id`::`String`; _mediaType=nothing) -> `Channel`{ `Nothing` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`BomApi`** | API context | 
**`bom_id`** | **`String`** |  |

### Return type

`Nothing`

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **get_bom**
> `get_bom`(_api::`BomApi`, `bom_id`::`String`; _mediaType=nothing) -> `Bom`, `OpenAPI.Clients.ApiResponse` <br/>
> `get_bom`(_api::`BomApi`, response_stream::`Channel`, `bom_id`::`String`; _mediaType=nothing) -> `Channel`{ `Bom` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`BomApi`** | API context | 
**`bom_id`** | **`String`** |  |

### Return type

[**`Bom`**](Bom.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **list_boms**
> `list_boms`(_api::`BomApi`; `page`=nothing, `page_size`=nothing, `search`=nothing, `product_id`=nothing, _mediaType=nothing) -> `Vector{Bom}`, `OpenAPI.Clients.ApiResponse` <br/>
> `list_boms`(_api::`BomApi`, response_stream::`Channel`; `page`=nothing, `page_size`=nothing, `search`=nothing, `product_id`=nothing, _mediaType=nothing) -> `Channel`{ `Vector{Bom}` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`BomApi`** | API context | 

### Optional Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **`page`** | **`Int64`** |  | [default to nothing]
 **`page_size`** | **`Int64`** |  | [default to nothing]
 **`search`** | **`String`** |  | [default to nothing]
 **`product_id`** | **`String`** | Filter by finished product id. | [default to nothing]

### Return type

[**`Vector{Bom}`**](Bom.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **update_bom**
> `update_bom`(_api::`BomApi`, `bom_id`::`String`, `bom_update`::`BomUpdate`; _mediaType=nothing) -> `Bom`, `OpenAPI.Clients.ApiResponse` <br/>
> `update_bom`(_api::`BomApi`, response_stream::`Channel`, `bom_id`::`String`, `bom_update`::`BomUpdate`; _mediaType=nothing) -> `Channel`{ `Bom` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`BomApi`** | API context | 
**`bom_id`** | **`String`** |  |
**`bom_update`** | [**`BomUpdate`**](BomUpdate.md) |  |

### Return type

[**`Bom`**](Bom.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

