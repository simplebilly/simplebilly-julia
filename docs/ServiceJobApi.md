# ServiceJobApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_service_job**](ServiceJobApi.md#create_service_job) | **POST** /api/v1/service-jobs | 
[**delete_service_job**](ServiceJobApi.md#delete_service_job) | **DELETE** /api/v1/service-jobs/{id} | 
[**get_service_job**](ServiceJobApi.md#get_service_job) | **GET** /api/v1/service-jobs/{id} | 
[**get_service_jobs**](ServiceJobApi.md#get_service_jobs) | **GET** /api/v1/service-jobs/ | 
[**update_service_job**](ServiceJobApi.md#update_service_job) | **PUT** /api/v1/service-jobs/{id} | 


# **create_service_job**
> `create_service_job`(_api::`ServiceJobApi`, `service_job_create`::`ServiceJobCreate`; _mediaType=nothing) -> `ServiceJob`, `OpenAPI.Clients.ApiResponse` <br/>
> `create_service_job`(_api::`ServiceJobApi`, response_stream::`Channel`, `service_job_create`::`ServiceJobCreate`; _mediaType=nothing) -> `Channel`{ `ServiceJob` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ServiceJobApi`** | API context | 
**`service_job_create`** | [**`ServiceJobCreate`**](ServiceJobCreate.md) |  |

### Return type

[**`ServiceJob`**](ServiceJob.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **delete_service_job**
> `delete_service_job`(_api::`ServiceJobApi`, `id`::`String`; _mediaType=nothing) -> `Nothing`, `OpenAPI.Clients.ApiResponse` <br/>
> `delete_service_job`(_api::`ServiceJobApi`, response_stream::`Channel`, `id`::`String`; _mediaType=nothing) -> `Channel`{ `Nothing` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ServiceJobApi`** | API context | 
**`id`** | **`String`** |  |

### Return type

`Nothing`

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **get_service_job**
> `get_service_job`(_api::`ServiceJobApi`, `id`::`String`; _mediaType=nothing) -> `ServiceJob`, `OpenAPI.Clients.ApiResponse` <br/>
> `get_service_job`(_api::`ServiceJobApi`, response_stream::`Channel`, `id`::`String`; _mediaType=nothing) -> `Channel`{ `ServiceJob` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ServiceJobApi`** | API context | 
**`id`** | **`String`** |  |

### Return type

[**`ServiceJob`**](ServiceJob.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **get_service_jobs**
> `get_service_jobs`(_api::`ServiceJobApi`; `page`=nothing, `page_size`=nothing, `search`=nothing, `include_deleted`=nothing, _mediaType=nothing) -> `Vector{ServiceJob}`, `OpenAPI.Clients.ApiResponse` <br/>
> `get_service_jobs`(_api::`ServiceJobApi`, response_stream::`Channel`; `page`=nothing, `page_size`=nothing, `search`=nothing, `include_deleted`=nothing, _mediaType=nothing) -> `Channel`{ `Vector{ServiceJob}` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ServiceJobApi`** | API context | 

### Optional Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **`page`** | **`Int64`** |  | [default to nothing]
 **`page_size`** | **`Int64`** |  | [default to nothing]
 **`search`** | **`String`** |  | [default to nothing]
 **`include_deleted`** | **`Bool`** | Soft-delete entities: set true to include rows with &#x60;deleted_at&#x60; set. | [default to nothing]

### Return type

[**`Vector{ServiceJob}`**](ServiceJob.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **update_service_job**
> `update_service_job`(_api::`ServiceJobApi`, `id`::`String`, `service_job_update`::`ServiceJobUpdate`; _mediaType=nothing) -> `ServiceJob`, `OpenAPI.Clients.ApiResponse` <br/>
> `update_service_job`(_api::`ServiceJobApi`, response_stream::`Channel`, `id`::`String`, `service_job_update`::`ServiceJobUpdate`; _mediaType=nothing) -> `Channel`{ `ServiceJob` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ServiceJobApi`** | API context | 
**`id`** | **`String`** |  |
**`service_job_update`** | [**`ServiceJobUpdate`**](ServiceJobUpdate.md) |  |

### Return type

[**`ServiceJob`**](ServiceJob.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

