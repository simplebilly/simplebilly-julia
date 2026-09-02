# TrainingsApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_my_trainings**](TrainingsApi.md#get_my_trainings) | **GET** /api/v1/trainings/me | 
[**get_training_content**](TrainingsApi.md#get_training_content) | **GET** /api/v1/trainings/content/{code} | 
[**get_training_overview**](TrainingsApi.md#get_training_overview) | **GET** /api/v1/trainings/overview | 
[**submit_training_result**](TrainingsApi.md#submit_training_result) | **POST** /api/v1/trainings/submit-result | 


# **get_my_trainings**
> `get_my_trainings`(_api::`TrainingsApi`; _mediaType=nothing) -> `Vector{MyTrainingItem}`, `OpenAPI.Clients.ApiResponse` <br/>
> `get_my_trainings`(_api::`TrainingsApi`, response_stream::`Channel`; _mediaType=nothing) -> `Channel`{ `Vector{MyTrainingItem}` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters
This endpoint does not need any parameter.

### Return type

[**`Vector{MyTrainingItem}`**](MyTrainingItem.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **get_training_content**
> `get_training_content`(_api::`TrainingsApi`, `code`::`String`; _mediaType=nothing) -> `TrainingContent`, `OpenAPI.Clients.ApiResponse` <br/>
> `get_training_content`(_api::`TrainingsApi`, response_stream::`Channel`, `code`::`String`; _mediaType=nothing) -> `Channel`{ `TrainingContent` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`TrainingsApi`** | API context | 
**`code`** | **`String`** | Training code, e.g. data_privacy |

### Return type

[**`TrainingContent`**](TrainingContent.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **get_training_overview**
> `get_training_overview`(_api::`TrainingsApi`; _mediaType=nothing) -> `Vector{HrTrainingOverview}`, `OpenAPI.Clients.ApiResponse` <br/>
> `get_training_overview`(_api::`TrainingsApi`, response_stream::`Channel`; _mediaType=nothing) -> `Channel`{ `Vector{HrTrainingOverview}` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters
This endpoint does not need any parameter.

### Return type

[**`Vector{HrTrainingOverview}`**](HrTrainingOverview.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **submit_training_result**
> `submit_training_result`(_api::`TrainingsApi`, `submit_result_dto`::`SubmitResultDto`; _mediaType=nothing) -> `SubmitResultResponse`, `OpenAPI.Clients.ApiResponse` <br/>
> `submit_training_result`(_api::`TrainingsApi`, response_stream::`Channel`, `submit_result_dto`::`SubmitResultDto`; _mediaType=nothing) -> `Channel`{ `SubmitResultResponse` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`TrainingsApi`** | API context | 
**`submit_result_dto`** | [**`SubmitResultDto`**](SubmitResultDto.md) |  |

### Return type

[**`SubmitResultResponse`**](SubmitResultResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

