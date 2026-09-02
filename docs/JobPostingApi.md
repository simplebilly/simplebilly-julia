# JobPostingApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_job_posting**](JobPostingApi.md#create_job_posting) | **POST** /api/v1/job-postings | 
[**delete_job_posting**](JobPostingApi.md#delete_job_posting) | **DELETE** /api/v1/job-postings/{id} | 
[**get_job_posting**](JobPostingApi.md#get_job_posting) | **GET** /api/v1/job-postings/{id} | 
[**list_job_postings**](JobPostingApi.md#list_job_postings) | **GET** /api/v1/job-postings | 
[**update_job_posting**](JobPostingApi.md#update_job_posting) | **PUT** /api/v1/job-postings/{id} | 


# **create_job_posting**
> `create_job_posting`(_api::`JobPostingApi`, `job_posting_create`::`JobPostingCreate`; _mediaType=nothing) -> `JobPosting`, `OpenAPI.Clients.ApiResponse` <br/>
> `create_job_posting`(_api::`JobPostingApi`, response_stream::`Channel`, `job_posting_create`::`JobPostingCreate`; _mediaType=nothing) -> `Channel`{ `JobPosting` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`JobPostingApi`** | API context | 
**`job_posting_create`** | [**`JobPostingCreate`**](JobPostingCreate.md) |  |

### Return type

[**`JobPosting`**](JobPosting.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **delete_job_posting**
> `delete_job_posting`(_api::`JobPostingApi`, `id`::`String`; _mediaType=nothing) -> `Nothing`, `OpenAPI.Clients.ApiResponse` <br/>
> `delete_job_posting`(_api::`JobPostingApi`, response_stream::`Channel`, `id`::`String`; _mediaType=nothing) -> `Channel`{ `Nothing` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`JobPostingApi`** | API context | 
**`id`** | **`String`** |  |

### Return type

`Nothing`

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **get_job_posting**
> `get_job_posting`(_api::`JobPostingApi`, `id`::`String`; _mediaType=nothing) -> `JobPosting`, `OpenAPI.Clients.ApiResponse` <br/>
> `get_job_posting`(_api::`JobPostingApi`, response_stream::`Channel`, `id`::`String`; _mediaType=nothing) -> `Channel`{ `JobPosting` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`JobPostingApi`** | API context | 
**`id`** | **`String`** |  |

### Return type

[**`JobPosting`**](JobPosting.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **list_job_postings**
> `list_job_postings`(_api::`JobPostingApi`; `status`=nothing, `page`=nothing, `page_size`=nothing, _mediaType=nothing) -> `Vector{JobPosting}`, `OpenAPI.Clients.ApiResponse` <br/>
> `list_job_postings`(_api::`JobPostingApi`, response_stream::`Channel`; `status`=nothing, `page`=nothing, `page_size`=nothing, _mediaType=nothing) -> `Channel`{ `Vector{JobPosting}` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`JobPostingApi`** | API context | 

### Optional Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **`status`** | **`String`** |  | [default to nothing]
 **`page`** | **`Int64`** |  | [default to nothing]
 **`page_size`** | **`Int64`** |  | [default to nothing]

### Return type

[**`Vector{JobPosting}`**](JobPosting.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **update_job_posting**
> `update_job_posting`(_api::`JobPostingApi`, `id`::`String`, `job_posting_update`::`JobPostingUpdate`; _mediaType=nothing) -> `JobPosting`, `OpenAPI.Clients.ApiResponse` <br/>
> `update_job_posting`(_api::`JobPostingApi`, response_stream::`Channel`, `id`::`String`, `job_posting_update`::`JobPostingUpdate`; _mediaType=nothing) -> `Channel`{ `JobPosting` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`JobPostingApi`** | API context | 
**`id`** | **`String`** |  |
**`job_posting_update`** | [**`JobPostingUpdate`**](JobPostingUpdate.md) |  |

### Return type

[**`JobPosting`**](JobPosting.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

