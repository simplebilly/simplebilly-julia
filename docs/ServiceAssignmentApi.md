# ServiceAssignmentApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_service_assignment**](ServiceAssignmentApi.md#create_service_assignment) | **POST** /api/v1/service-assignments | 
[**delete_service_assignment**](ServiceAssignmentApi.md#delete_service_assignment) | **DELETE** /api/v1/service-assignments/{id} | 
[**get_service_assignment**](ServiceAssignmentApi.md#get_service_assignment) | **GET** /api/v1/service-assignments/{id} | 
[**get_service_assignments**](ServiceAssignmentApi.md#get_service_assignments) | **GET** /api/v1/service-assignments/ | 
[**update_service_assignment**](ServiceAssignmentApi.md#update_service_assignment) | **PUT** /api/v1/service-assignments/{id} | 


# **create_service_assignment**
> `create_service_assignment`(_api::`ServiceAssignmentApi`, `service_assignment_create`::`ServiceAssignmentCreate`; _mediaType=nothing) -> `ServiceAssignment`, `OpenAPI.Clients.ApiResponse` <br/>
> `create_service_assignment`(_api::`ServiceAssignmentApi`, response_stream::`Channel`, `service_assignment_create`::`ServiceAssignmentCreate`; _mediaType=nothing) -> `Channel`{ `ServiceAssignment` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ServiceAssignmentApi`** | API context | 
**`service_assignment_create`** | [**`ServiceAssignmentCreate`**](ServiceAssignmentCreate.md) |  |

### Return type

[**`ServiceAssignment`**](ServiceAssignment.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **delete_service_assignment**
> `delete_service_assignment`(_api::`ServiceAssignmentApi`, `id`::`String`; _mediaType=nothing) -> `Nothing`, `OpenAPI.Clients.ApiResponse` <br/>
> `delete_service_assignment`(_api::`ServiceAssignmentApi`, response_stream::`Channel`, `id`::`String`; _mediaType=nothing) -> `Channel`{ `Nothing` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ServiceAssignmentApi`** | API context | 
**`id`** | **`String`** |  |

### Return type

`Nothing`

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **get_service_assignment**
> `get_service_assignment`(_api::`ServiceAssignmentApi`, `id`::`String`; _mediaType=nothing) -> `ServiceAssignment`, `OpenAPI.Clients.ApiResponse` <br/>
> `get_service_assignment`(_api::`ServiceAssignmentApi`, response_stream::`Channel`, `id`::`String`; _mediaType=nothing) -> `Channel`{ `ServiceAssignment` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ServiceAssignmentApi`** | API context | 
**`id`** | **`String`** |  |

### Return type

[**`ServiceAssignment`**](ServiceAssignment.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **get_service_assignments**
> `get_service_assignments`(_api::`ServiceAssignmentApi`; `page`=nothing, `page_size`=nothing, `search`=nothing, `include_deleted`=nothing, _mediaType=nothing) -> `Vector{ServiceAssignment}`, `OpenAPI.Clients.ApiResponse` <br/>
> `get_service_assignments`(_api::`ServiceAssignmentApi`, response_stream::`Channel`; `page`=nothing, `page_size`=nothing, `search`=nothing, `include_deleted`=nothing, _mediaType=nothing) -> `Channel`{ `Vector{ServiceAssignment}` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ServiceAssignmentApi`** | API context | 

### Optional Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **`page`** | **`Int64`** |  | [default to nothing]
 **`page_size`** | **`Int64`** |  | [default to nothing]
 **`search`** | **`String`** |  | [default to nothing]
 **`include_deleted`** | **`Bool`** | Soft-delete entities: set true to include rows with &#x60;deleted_at&#x60; set. | [default to nothing]

### Return type

[**`Vector{ServiceAssignment}`**](ServiceAssignment.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **update_service_assignment**
> `update_service_assignment`(_api::`ServiceAssignmentApi`, `id`::`String`, `service_assignment_update`::`ServiceAssignmentUpdate`; _mediaType=nothing) -> `ServiceAssignment`, `OpenAPI.Clients.ApiResponse` <br/>
> `update_service_assignment`(_api::`ServiceAssignmentApi`, response_stream::`Channel`, `id`::`String`, `service_assignment_update`::`ServiceAssignmentUpdate`; _mediaType=nothing) -> `Channel`{ `ServiceAssignment` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ServiceAssignmentApi`** | API context | 
**`id`** | **`String`** |  |
**`service_assignment_update`** | [**`ServiceAssignmentUpdate`**](ServiceAssignmentUpdate.md) |  |

### Return type

[**`ServiceAssignment`**](ServiceAssignment.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

