# AiApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ai_suggest_api**](AiApi.md#ai_suggest_api) | **POST** /api/v1/support/ai/suggest | 
[**create_worker_api**](AiApi.md#create_worker_api) | **POST** /api/v1/support/ai/workers | 
[**list_workers_api**](AiApi.md#list_workers_api) | **GET** /api/v1/support/ai/workers | 
[**run_worker_api**](AiApi.md#run_worker_api) | **POST** /api/v1/support/ai/workers/{worker_id}/run | 


# **ai_suggest_api**
> `ai_suggest_api`(_api::`AiApi`, `ai_suggestion_request`::`AiSuggestionRequest`; _mediaType=nothing) -> `AiSuggestion`, `OpenAPI.Clients.ApiResponse` <br/>
> `ai_suggest_api`(_api::`AiApi`, response_stream::`Channel`, `ai_suggestion_request`::`AiSuggestionRequest`; _mediaType=nothing) -> `Channel`{ `AiSuggestion` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`AiApi`** | API context | 
**`ai_suggestion_request`** | [**`AiSuggestionRequest`**](AiSuggestionRequest.md) |  |

### Return type

[**`AiSuggestion`**](AiSuggestion.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **create_worker_api**
> `create_worker_api`(_api::`AiApi`, `ai_config_dto`::`AiConfigDto`; _mediaType=nothing) -> `AiWorkerConfig`, `OpenAPI.Clients.ApiResponse` <br/>
> `create_worker_api`(_api::`AiApi`, response_stream::`Channel`, `ai_config_dto`::`AiConfigDto`; _mediaType=nothing) -> `Channel`{ `AiWorkerConfig` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`AiApi`** | API context | 
**`ai_config_dto`** | [**`AiConfigDto`**](AiConfigDto.md) |  |

### Return type

[**`AiWorkerConfig`**](AiWorkerConfig.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **list_workers_api**
> `list_workers_api`(_api::`AiApi`; _mediaType=nothing) -> `Vector{AiWorkerConfig}`, `OpenAPI.Clients.ApiResponse` <br/>
> `list_workers_api`(_api::`AiApi`, response_stream::`Channel`; _mediaType=nothing) -> `Channel`{ `Vector{AiWorkerConfig}` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters
This endpoint does not need any parameter.

### Return type

[**`Vector{AiWorkerConfig}`**](AiWorkerConfig.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **run_worker_api**
> `run_worker_api`(_api::`AiApi`, `worker_id`::`String`, `ai_suggestion_request`::`AiSuggestionRequest`; _mediaType=nothing) -> `AiSuggestion`, `OpenAPI.Clients.ApiResponse` <br/>
> `run_worker_api`(_api::`AiApi`, response_stream::`Channel`, `worker_id`::`String`, `ai_suggestion_request`::`AiSuggestionRequest`; _mediaType=nothing) -> `Channel`{ `AiSuggestion` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`AiApi`** | API context | 
**`worker_id`** | **`String`** |  |
**`ai_suggestion_request`** | [**`AiSuggestionRequest`**](AiSuggestionRequest.md) |  |

### Return type

[**`AiSuggestion`**](AiSuggestion.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

