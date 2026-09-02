# ImportRunnerApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_import_status**](ImportRunnerApi.md#get_import_status) | **GET** /api/v1/import/{job_id} | 
[**start_import**](ImportRunnerApi.md#start_import) | **POST** /api/v1/import/start | 
[**test_import_connection**](ImportRunnerApi.md#test_import_connection) | **POST** /api/v1/import/test | 


# **get_import_status**
> `get_import_status`(_api::`ImportRunnerApi`, `job_id`::`String`; _mediaType=nothing) -> `ImportJobStatus`, `OpenAPI.Clients.ApiResponse` <br/>
> `get_import_status`(_api::`ImportRunnerApi`, response_stream::`Channel`, `job_id`::`String`; _mediaType=nothing) -> `Channel`{ `ImportJobStatus` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ImportRunnerApi`** | API context | 
**`job_id`** | **`String`** |  |

### Return type

[**`ImportJobStatus`**](ImportJobStatus.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **start_import**
> `start_import`(_api::`ImportRunnerApi`, `import_start_request`::`ImportStartRequest`; _mediaType=nothing) -> `ImportStartResponse`, `OpenAPI.Clients.ApiResponse` <br/>
> `start_import`(_api::`ImportRunnerApi`, response_stream::`Channel`, `import_start_request`::`ImportStartRequest`; _mediaType=nothing) -> `Channel`{ `ImportStartResponse` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ImportRunnerApi`** | API context | 
**`import_start_request`** | [**`ImportStartRequest`**](ImportStartRequest.md) |  |

### Return type

[**`ImportStartResponse`**](ImportStartResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **test_import_connection**
> `test_import_connection`(_api::`ImportRunnerApi`, `import_test_request`::`ImportTestRequest`; _mediaType=nothing) -> `ImportTestResponse`, `OpenAPI.Clients.ApiResponse` <br/>
> `test_import_connection`(_api::`ImportRunnerApi`, response_stream::`Channel`, `import_test_request`::`ImportTestRequest`; _mediaType=nothing) -> `Channel`{ `ImportTestResponse` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ImportRunnerApi`** | API context | 
**`import_test_request`** | [**`ImportTestRequest`**](ImportTestRequest.md) |  |

### Return type

[**`ImportTestResponse`**](ImportTestResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

