# ComplianceTrainingApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_compliance_training**](ComplianceTrainingApi.md#create_compliance_training) | **POST** /api/v1/compliance-trainings | 
[**delete_compliance_training**](ComplianceTrainingApi.md#delete_compliance_training) | **DELETE** /api/v1/compliance-trainings/{id} | 
[**get_compliance_training**](ComplianceTrainingApi.md#get_compliance_training) | **GET** /api/v1/compliance-trainings/{id} | 
[**get_compliance_trainings**](ComplianceTrainingApi.md#get_compliance_trainings) | **GET** /api/v1/compliance-trainings/ | 
[**update_compliance_training**](ComplianceTrainingApi.md#update_compliance_training) | **PUT** /api/v1/compliance-trainings/{id} | 


# **create_compliance_training**
> `create_compliance_training`(_api::`ComplianceTrainingApi`, `compliance_training_create`::`ComplianceTrainingCreate`; _mediaType=nothing) -> `ComplianceTraining`, `OpenAPI.Clients.ApiResponse` <br/>
> `create_compliance_training`(_api::`ComplianceTrainingApi`, response_stream::`Channel`, `compliance_training_create`::`ComplianceTrainingCreate`; _mediaType=nothing) -> `Channel`{ `ComplianceTraining` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ComplianceTrainingApi`** | API context | 
**`compliance_training_create`** | [**`ComplianceTrainingCreate`**](ComplianceTrainingCreate.md) |  |

### Return type

[**`ComplianceTraining`**](ComplianceTraining.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **delete_compliance_training**
> `delete_compliance_training`(_api::`ComplianceTrainingApi`, `id`::`String`; _mediaType=nothing) -> `Nothing`, `OpenAPI.Clients.ApiResponse` <br/>
> `delete_compliance_training`(_api::`ComplianceTrainingApi`, response_stream::`Channel`, `id`::`String`; _mediaType=nothing) -> `Channel`{ `Nothing` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ComplianceTrainingApi`** | API context | 
**`id`** | **`String`** |  |

### Return type

`Nothing`

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **get_compliance_training**
> `get_compliance_training`(_api::`ComplianceTrainingApi`, `id`::`String`; _mediaType=nothing) -> `ComplianceTraining`, `OpenAPI.Clients.ApiResponse` <br/>
> `get_compliance_training`(_api::`ComplianceTrainingApi`, response_stream::`Channel`, `id`::`String`; _mediaType=nothing) -> `Channel`{ `ComplianceTraining` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ComplianceTrainingApi`** | API context | 
**`id`** | **`String`** |  |

### Return type

[**`ComplianceTraining`**](ComplianceTraining.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **get_compliance_trainings**
> `get_compliance_trainings`(_api::`ComplianceTrainingApi`; `page`=nothing, `page_size`=nothing, `search`=nothing, `include_deleted`=nothing, _mediaType=nothing) -> `Vector{ComplianceTraining}`, `OpenAPI.Clients.ApiResponse` <br/>
> `get_compliance_trainings`(_api::`ComplianceTrainingApi`, response_stream::`Channel`; `page`=nothing, `page_size`=nothing, `search`=nothing, `include_deleted`=nothing, _mediaType=nothing) -> `Channel`{ `Vector{ComplianceTraining}` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ComplianceTrainingApi`** | API context | 

### Optional Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **`page`** | **`Int64`** |  | [default to nothing]
 **`page_size`** | **`Int64`** |  | [default to nothing]
 **`search`** | **`String`** |  | [default to nothing]
 **`include_deleted`** | **`Bool`** | Soft-delete entities: set true to include rows with &#x60;deleted_at&#x60; set. | [default to nothing]

### Return type

[**`Vector{ComplianceTraining}`**](ComplianceTraining.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **update_compliance_training**
> `update_compliance_training`(_api::`ComplianceTrainingApi`, `id`::`String`, `compliance_training_update`::`ComplianceTrainingUpdate`; _mediaType=nothing) -> `ComplianceTraining`, `OpenAPI.Clients.ApiResponse` <br/>
> `update_compliance_training`(_api::`ComplianceTrainingApi`, response_stream::`Channel`, `id`::`String`, `compliance_training_update`::`ComplianceTrainingUpdate`; _mediaType=nothing) -> `Channel`{ `ComplianceTraining` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ComplianceTrainingApi`** | API context | 
**`id`** | **`String`** |  |
**`compliance_training_update`** | [**`ComplianceTrainingUpdate`**](ComplianceTrainingUpdate.md) |  |

### Return type

[**`ComplianceTraining`**](ComplianceTraining.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

