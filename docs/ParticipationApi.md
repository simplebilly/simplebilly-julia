# ParticipationApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_participation**](ParticipationApi.md#create_participation) | **POST** /api/v1/participations | 
[**delete_participation**](ParticipationApi.md#delete_participation) | **DELETE** /api/v1/participations/{id} | 
[**get_participation**](ParticipationApi.md#get_participation) | **GET** /api/v1/participations/{id} | 
[**get_participations**](ParticipationApi.md#get_participations) | **GET** /api/v1/participations/ | 
[**update_participation**](ParticipationApi.md#update_participation) | **PUT** /api/v1/participations/{id} | 


# **create_participation**
> `create_participation`(_api::`ParticipationApi`, `participation_create`::`ParticipationCreate`; _mediaType=nothing) -> `Participation`, `OpenAPI.Clients.ApiResponse` <br/>
> `create_participation`(_api::`ParticipationApi`, response_stream::`Channel`, `participation_create`::`ParticipationCreate`; _mediaType=nothing) -> `Channel`{ `Participation` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ParticipationApi`** | API context | 
**`participation_create`** | [**`ParticipationCreate`**](ParticipationCreate.md) |  |

### Return type

[**`Participation`**](Participation.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **delete_participation**
> `delete_participation`(_api::`ParticipationApi`, `id`::`String`; _mediaType=nothing) -> `Nothing`, `OpenAPI.Clients.ApiResponse` <br/>
> `delete_participation`(_api::`ParticipationApi`, response_stream::`Channel`, `id`::`String`; _mediaType=nothing) -> `Channel`{ `Nothing` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ParticipationApi`** | API context | 
**`id`** | **`String`** |  |

### Return type

`Nothing`

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **get_participation**
> `get_participation`(_api::`ParticipationApi`, `id`::`String`; _mediaType=nothing) -> `Participation`, `OpenAPI.Clients.ApiResponse` <br/>
> `get_participation`(_api::`ParticipationApi`, response_stream::`Channel`, `id`::`String`; _mediaType=nothing) -> `Channel`{ `Participation` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ParticipationApi`** | API context | 
**`id`** | **`String`** |  |

### Return type

[**`Participation`**](Participation.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **get_participations**
> `get_participations`(_api::`ParticipationApi`; `page`=nothing, `page_size`=nothing, `search`=nothing, `include_deleted`=nothing, _mediaType=nothing) -> `Vector{Participation}`, `OpenAPI.Clients.ApiResponse` <br/>
> `get_participations`(_api::`ParticipationApi`, response_stream::`Channel`; `page`=nothing, `page_size`=nothing, `search`=nothing, `include_deleted`=nothing, _mediaType=nothing) -> `Channel`{ `Vector{Participation}` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ParticipationApi`** | API context | 

### Optional Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **`page`** | **`Int64`** |  | [default to nothing]
 **`page_size`** | **`Int64`** |  | [default to nothing]
 **`search`** | **`String`** |  | [default to nothing]
 **`include_deleted`** | **`Bool`** | Soft-delete entities: set true to include rows with &#x60;deleted_at&#x60; set. | [default to nothing]

### Return type

[**`Vector{Participation}`**](Participation.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **update_participation**
> `update_participation`(_api::`ParticipationApi`, `id`::`String`, `participation_update`::`ParticipationUpdate`; _mediaType=nothing) -> `Participation`, `OpenAPI.Clients.ApiResponse` <br/>
> `update_participation`(_api::`ParticipationApi`, response_stream::`Channel`, `id`::`String`, `participation_update`::`ParticipationUpdate`; _mediaType=nothing) -> `Channel`{ `Participation` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ParticipationApi`** | API context | 
**`id`** | **`String`** |  |
**`participation_update`** | [**`ParticipationUpdate`**](ParticipationUpdate.md) |  |

### Return type

[**`Participation`**](Participation.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

