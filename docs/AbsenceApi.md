# AbsenceApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_absence**](AbsenceApi.md#create_absence) | **POST** /api/v1/absences | 
[**delete_absence**](AbsenceApi.md#delete_absence) | **DELETE** /api/v1/absences/{id} | 
[**get_absence**](AbsenceApi.md#get_absence) | **GET** /api/v1/absences/{id} | 
[**get_absences**](AbsenceApi.md#get_absences) | **GET** /api/v1/absences/ | 
[**update_absence**](AbsenceApi.md#update_absence) | **PUT** /api/v1/absences/{id} | 


# **create_absence**
> `create_absence`(_api::`AbsenceApi`, `absence_create`::`AbsenceCreate`; _mediaType=nothing) -> `Absence`, `OpenAPI.Clients.ApiResponse` <br/>
> `create_absence`(_api::`AbsenceApi`, response_stream::`Channel`, `absence_create`::`AbsenceCreate`; _mediaType=nothing) -> `Channel`{ `Absence` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`AbsenceApi`** | API context | 
**`absence_create`** | [**`AbsenceCreate`**](AbsenceCreate.md) |  |

### Return type

[**`Absence`**](Absence.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **delete_absence**
> `delete_absence`(_api::`AbsenceApi`, `id`::`String`; _mediaType=nothing) -> `Nothing`, `OpenAPI.Clients.ApiResponse` <br/>
> `delete_absence`(_api::`AbsenceApi`, response_stream::`Channel`, `id`::`String`; _mediaType=nothing) -> `Channel`{ `Nothing` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`AbsenceApi`** | API context | 
**`id`** | **`String`** |  |

### Return type

`Nothing`

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **get_absence**
> `get_absence`(_api::`AbsenceApi`, `id`::`String`; _mediaType=nothing) -> `Absence`, `OpenAPI.Clients.ApiResponse` <br/>
> `get_absence`(_api::`AbsenceApi`, response_stream::`Channel`, `id`::`String`; _mediaType=nothing) -> `Channel`{ `Absence` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`AbsenceApi`** | API context | 
**`id`** | **`String`** |  |

### Return type

[**`Absence`**](Absence.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **get_absences**
> `get_absences`(_api::`AbsenceApi`; `page`=nothing, `page_size`=nothing, `search`=nothing, `include_deleted`=nothing, _mediaType=nothing) -> `Vector{Absence}`, `OpenAPI.Clients.ApiResponse` <br/>
> `get_absences`(_api::`AbsenceApi`, response_stream::`Channel`; `page`=nothing, `page_size`=nothing, `search`=nothing, `include_deleted`=nothing, _mediaType=nothing) -> `Channel`{ `Vector{Absence}` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`AbsenceApi`** | API context | 

### Optional Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **`page`** | **`Int64`** |  | [default to nothing]
 **`page_size`** | **`Int64`** |  | [default to nothing]
 **`search`** | **`String`** |  | [default to nothing]
 **`include_deleted`** | **`Bool`** | Soft-delete entities: set true to include rows with &#x60;deleted_at&#x60; set. | [default to nothing]

### Return type

[**`Vector{Absence}`**](Absence.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **update_absence**
> `update_absence`(_api::`AbsenceApi`, `id`::`String`, `absence_update`::`AbsenceUpdate`; _mediaType=nothing) -> `Absence`, `OpenAPI.Clients.ApiResponse` <br/>
> `update_absence`(_api::`AbsenceApi`, response_stream::`Channel`, `id`::`String`, `absence_update`::`AbsenceUpdate`; _mediaType=nothing) -> `Channel`{ `Absence` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`AbsenceApi`** | API context | 
**`id`** | **`String`** |  |
**`absence_update`** | [**`AbsenceUpdate`**](AbsenceUpdate.md) |  |

### Return type

[**`Absence`**](Absence.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

