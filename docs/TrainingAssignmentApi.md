# TrainingAssignmentApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_training_assignment**](TrainingAssignmentApi.md#create_training_assignment) | **POST** /api/v1/training-assignments | 
[**delete_training_assignment**](TrainingAssignmentApi.md#delete_training_assignment) | **DELETE** /api/v1/training-assignments/{id} | 
[**get_training_assignment**](TrainingAssignmentApi.md#get_training_assignment) | **GET** /api/v1/training-assignments/{id} | 
[**get_training_assignments**](TrainingAssignmentApi.md#get_training_assignments) | **GET** /api/v1/training-assignments/ | 
[**update_training_assignment**](TrainingAssignmentApi.md#update_training_assignment) | **PUT** /api/v1/training-assignments/{id} | 


# **create_training_assignment**
> `create_training_assignment`(_api::`TrainingAssignmentApi`, `training_assignment_create`::`TrainingAssignmentCreate`; _mediaType=nothing) -> `TrainingAssignment`, `OpenAPI.Clients.ApiResponse` <br/>
> `create_training_assignment`(_api::`TrainingAssignmentApi`, response_stream::`Channel`, `training_assignment_create`::`TrainingAssignmentCreate`; _mediaType=nothing) -> `Channel`{ `TrainingAssignment` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`TrainingAssignmentApi`** | API context | 
**`training_assignment_create`** | [**`TrainingAssignmentCreate`**](TrainingAssignmentCreate.md) |  |

### Return type

[**`TrainingAssignment`**](TrainingAssignment.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **delete_training_assignment**
> `delete_training_assignment`(_api::`TrainingAssignmentApi`, `id`::`String`; _mediaType=nothing) -> `Nothing`, `OpenAPI.Clients.ApiResponse` <br/>
> `delete_training_assignment`(_api::`TrainingAssignmentApi`, response_stream::`Channel`, `id`::`String`; _mediaType=nothing) -> `Channel`{ `Nothing` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`TrainingAssignmentApi`** | API context | 
**`id`** | **`String`** |  |

### Return type

`Nothing`

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **get_training_assignment**
> `get_training_assignment`(_api::`TrainingAssignmentApi`, `id`::`String`; _mediaType=nothing) -> `TrainingAssignment`, `OpenAPI.Clients.ApiResponse` <br/>
> `get_training_assignment`(_api::`TrainingAssignmentApi`, response_stream::`Channel`, `id`::`String`; _mediaType=nothing) -> `Channel`{ `TrainingAssignment` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`TrainingAssignmentApi`** | API context | 
**`id`** | **`String`** |  |

### Return type

[**`TrainingAssignment`**](TrainingAssignment.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **get_training_assignments**
> `get_training_assignments`(_api::`TrainingAssignmentApi`; `page`=nothing, `page_size`=nothing, `search`=nothing, `include_deleted`=nothing, _mediaType=nothing) -> `Vector{TrainingAssignment}`, `OpenAPI.Clients.ApiResponse` <br/>
> `get_training_assignments`(_api::`TrainingAssignmentApi`, response_stream::`Channel`; `page`=nothing, `page_size`=nothing, `search`=nothing, `include_deleted`=nothing, _mediaType=nothing) -> `Channel`{ `Vector{TrainingAssignment}` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`TrainingAssignmentApi`** | API context | 

### Optional Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **`page`** | **`Int64`** |  | [default to nothing]
 **`page_size`** | **`Int64`** |  | [default to nothing]
 **`search`** | **`String`** |  | [default to nothing]
 **`include_deleted`** | **`Bool`** | Soft-delete entities: set true to include rows with &#x60;deleted_at&#x60; set. | [default to nothing]

### Return type

[**`Vector{TrainingAssignment}`**](TrainingAssignment.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **update_training_assignment**
> `update_training_assignment`(_api::`TrainingAssignmentApi`, `id`::`String`, `training_assignment_update`::`TrainingAssignmentUpdate`; _mediaType=nothing) -> `TrainingAssignment`, `OpenAPI.Clients.ApiResponse` <br/>
> `update_training_assignment`(_api::`TrainingAssignmentApi`, response_stream::`Channel`, `id`::`String`, `training_assignment_update`::`TrainingAssignmentUpdate`; _mediaType=nothing) -> `Channel`{ `TrainingAssignment` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`TrainingAssignmentApi`** | API context | 
**`id`** | **`String`** |  |
**`training_assignment_update`** | [**`TrainingAssignmentUpdate`**](TrainingAssignmentUpdate.md) |  |

### Return type

[**`TrainingAssignment`**](TrainingAssignment.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

