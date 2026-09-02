# DeclarationApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_declaration**](DeclarationApi.md#create_declaration) | **POST** /api/v1/declarations | 
[**declaration_restore**](DeclarationApi.md#declaration_restore) | **POST** /api/v1/declarations/{id}/restore | 
[**delete_declaration**](DeclarationApi.md#delete_declaration) | **DELETE** /api/v1/declarations/{id} | 
[**get_declaration**](DeclarationApi.md#get_declaration) | **GET** /api/v1/declarations/{id} | 
[**get_declarations**](DeclarationApi.md#get_declarations) | **GET** /api/v1/declarations/ | 
[**update_declaration**](DeclarationApi.md#update_declaration) | **PUT** /api/v1/declarations/{id} | 


# **create_declaration**
> `create_declaration`(_api::`DeclarationApi`, `declaration_create`::`DeclarationCreate`; _mediaType=nothing) -> `Declaration`, `OpenAPI.Clients.ApiResponse` <br/>
> `create_declaration`(_api::`DeclarationApi`, response_stream::`Channel`, `declaration_create`::`DeclarationCreate`; _mediaType=nothing) -> `Channel`{ `Declaration` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`DeclarationApi`** | API context | 
**`declaration_create`** | [**`DeclarationCreate`**](DeclarationCreate.md) |  |

### Return type

[**`Declaration`**](Declaration.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **declaration_restore**
> `declaration_restore`(_api::`DeclarationApi`, `id`::`String`; _mediaType=nothing) -> `Declaration`, `OpenAPI.Clients.ApiResponse` <br/>
> `declaration_restore`(_api::`DeclarationApi`, response_stream::`Channel`, `id`::`String`; _mediaType=nothing) -> `Channel`{ `Declaration` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`DeclarationApi`** | API context | 
**`id`** | **`String`** |  |

### Return type

[**`Declaration`**](Declaration.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **delete_declaration**
> `delete_declaration`(_api::`DeclarationApi`, `id`::`String`; _mediaType=nothing) -> `Nothing`, `OpenAPI.Clients.ApiResponse` <br/>
> `delete_declaration`(_api::`DeclarationApi`, response_stream::`Channel`, `id`::`String`; _mediaType=nothing) -> `Channel`{ `Nothing` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`DeclarationApi`** | API context | 
**`id`** | **`String`** |  |

### Return type

`Nothing`

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **get_declaration**
> `get_declaration`(_api::`DeclarationApi`, `id`::`String`; _mediaType=nothing) -> `Declaration`, `OpenAPI.Clients.ApiResponse` <br/>
> `get_declaration`(_api::`DeclarationApi`, response_stream::`Channel`, `id`::`String`; _mediaType=nothing) -> `Channel`{ `Declaration` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`DeclarationApi`** | API context | 
**`id`** | **`String`** |  |

### Return type

[**`Declaration`**](Declaration.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **get_declarations**
> `get_declarations`(_api::`DeclarationApi`; `page`=nothing, `page_size`=nothing, `search`=nothing, `include_deleted`=nothing, _mediaType=nothing) -> `Vector{Declaration}`, `OpenAPI.Clients.ApiResponse` <br/>
> `get_declarations`(_api::`DeclarationApi`, response_stream::`Channel`; `page`=nothing, `page_size`=nothing, `search`=nothing, `include_deleted`=nothing, _mediaType=nothing) -> `Channel`{ `Vector{Declaration}` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`DeclarationApi`** | API context | 

### Optional Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **`page`** | **`Int64`** |  | [default to nothing]
 **`page_size`** | **`Int64`** |  | [default to nothing]
 **`search`** | **`String`** |  | [default to nothing]
 **`include_deleted`** | **`Bool`** | Soft-delete entities: set true to include rows with &#x60;deleted_at&#x60; set. | [default to nothing]

### Return type

[**`Vector{Declaration}`**](Declaration.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **update_declaration**
> `update_declaration`(_api::`DeclarationApi`, `id`::`String`, `declaration_update`::`DeclarationUpdate`; _mediaType=nothing) -> `Declaration`, `OpenAPI.Clients.ApiResponse` <br/>
> `update_declaration`(_api::`DeclarationApi`, response_stream::`Channel`, `id`::`String`, `declaration_update`::`DeclarationUpdate`; _mediaType=nothing) -> `Channel`{ `Declaration` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`DeclarationApi`** | API context | 
**`id`** | **`String`** |  |
**`declaration_update`** | [**`DeclarationUpdate`**](DeclarationUpdate.md) |  |

### Return type

[**`Declaration`**](Declaration.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

