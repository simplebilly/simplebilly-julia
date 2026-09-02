# JobApplicationApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**apply_public**](JobApplicationApi.md#apply_public) | **POST** /api/v1/public/jobs/{posting_id}/apply | 
[**delete_job_application**](JobApplicationApi.md#delete_job_application) | **DELETE** /api/v1/job-applications/{application_id} | 
[**download_cv**](JobApplicationApi.md#download_cv) | **GET** /api/v1/job-applications/{application_id}/cv | 
[**get_job_application**](JobApplicationApi.md#get_job_application) | **GET** /api/v1/job-applications/{application_id} | 
[**inbound_email**](JobApplicationApi.md#inbound_email) | **POST** /api/v1/public/jobs/inbound-email | Inbound CV email, mailgun/sendgrid inbound-parse style: multipart form with &#x60;from&#x60;, &#x60;subject&#x60;, &#x60;body-plain&#x60; and one or more &#x60;attachment-N&#x60; file fields. The subject may reference a posting as &#x60;[JOB-&lt;posting_id&gt;]&#x60;; without one the application lands in the general inbox.
[**list_job_applications**](JobApplicationApi.md#list_job_applications) | **GET** /api/v1/job-applications | 
[**list_public_postings**](JobApplicationApi.md#list_public_postings) | **GET** /api/v1/public/jobs | 
[**score_job_application**](JobApplicationApi.md#score_job_application) | **POST** /api/v1/job-applications/{application_id}/score | 
[**update_job_application_status**](JobApplicationApi.md#update_job_application_status) | **PATCH** /api/v1/job-applications/{application_id}/status | 


# **apply_public**
> `apply_public`(_api::`JobApplicationApi`, `posting_id`::`String`; _mediaType=nothing) -> `Nothing`, `OpenAPI.Clients.ApiResponse` <br/>
> `apply_public`(_api::`JobApplicationApi`, response_stream::`Channel`, `posting_id`::`String`; _mediaType=nothing) -> `Channel`{ `Nothing` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`JobApplicationApi`** | API context | 
**`posting_id`** | **`String`** |  |

### Return type

`Nothing`

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **delete_job_application**
> `delete_job_application`(_api::`JobApplicationApi`, `application_id`::`String`; _mediaType=nothing) -> `JobApplication`, `OpenAPI.Clients.ApiResponse` <br/>
> `delete_job_application`(_api::`JobApplicationApi`, response_stream::`Channel`, `application_id`::`String`; _mediaType=nothing) -> `Channel`{ `JobApplication` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`JobApplicationApi`** | API context | 
**`application_id`** | **`String`** |  |

### Return type

[**`JobApplication`**](JobApplication.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **download_cv**
> `download_cv`(_api::`JobApplicationApi`, `application_id`::`String`; _mediaType=nothing) -> `Nothing`, `OpenAPI.Clients.ApiResponse` <br/>
> `download_cv`(_api::`JobApplicationApi`, response_stream::`Channel`, `application_id`::`String`; _mediaType=nothing) -> `Channel`{ `Nothing` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`JobApplicationApi`** | API context | 
**`application_id`** | **`String`** |  |

### Return type

`Nothing`

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **get_job_application**
> `get_job_application`(_api::`JobApplicationApi`, `application_id`::`String`; _mediaType=nothing) -> `JobApplication`, `OpenAPI.Clients.ApiResponse` <br/>
> `get_job_application`(_api::`JobApplicationApi`, response_stream::`Channel`, `application_id`::`String`; _mediaType=nothing) -> `Channel`{ `JobApplication` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`JobApplicationApi`** | API context | 
**`application_id`** | **`String`** |  |

### Return type

[**`JobApplication`**](JobApplication.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **inbound_email**
> `inbound_email`(_api::`JobApplicationApi`; _mediaType=nothing) -> `Nothing`, `OpenAPI.Clients.ApiResponse` <br/>
> `inbound_email`(_api::`JobApplicationApi`, response_stream::`Channel`; _mediaType=nothing) -> `Channel`{ `Nothing` }, `OpenAPI.Clients.ApiResponse`

Inbound CV email, mailgun/sendgrid inbound-parse style: multipart form with `from`, `subject`, `body-plain` and one or more `attachment-N` file fields. The subject may reference a posting as `[JOB-<posting_id>]`; without one the application lands in the general inbox.

### Required Parameters
This endpoint does not need any parameter.

### Return type

`Nothing`

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **list_job_applications**
> `list_job_applications`(_api::`JobApplicationApi`; `posting_id`=nothing, `status`=nothing, `page`=nothing, `page_size`=nothing, _mediaType=nothing) -> `Vector{JobApplication}`, `OpenAPI.Clients.ApiResponse` <br/>
> `list_job_applications`(_api::`JobApplicationApi`, response_stream::`Channel`; `posting_id`=nothing, `status`=nothing, `page`=nothing, `page_size`=nothing, _mediaType=nothing) -> `Channel`{ `Vector{JobApplication}` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`JobApplicationApi`** | API context | 

### Optional Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **`posting_id`** | **`String`** |  | [default to nothing]
 **`status`** | **`String`** |  | [default to nothing]
 **`page`** | **`Int64`** |  | [default to nothing]
 **`page_size`** | **`Int64`** |  | [default to nothing]

### Return type

[**`Vector{JobApplication}`**](JobApplication.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **list_public_postings**
> `list_public_postings`(_api::`JobApplicationApi`; _mediaType=nothing) -> `Vector{PublicPosting}`, `OpenAPI.Clients.ApiResponse` <br/>
> `list_public_postings`(_api::`JobApplicationApi`, response_stream::`Channel`; _mediaType=nothing) -> `Channel`{ `Vector{PublicPosting}` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters
This endpoint does not need any parameter.

### Return type

[**`Vector{PublicPosting}`**](PublicPosting.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **score_job_application**
> `score_job_application`(_api::`JobApplicationApi`, `application_id`::`String`; _mediaType=nothing) -> `JobApplication`, `OpenAPI.Clients.ApiResponse` <br/>
> `score_job_application`(_api::`JobApplicationApi`, response_stream::`Channel`, `application_id`::`String`; _mediaType=nothing) -> `Channel`{ `JobApplication` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`JobApplicationApi`** | API context | 
**`application_id`** | **`String`** |  |

### Return type

[**`JobApplication`**](JobApplication.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **update_job_application_status**
> `update_job_application_status`(_api::`JobApplicationApi`, `application_id`::`String`, `application_status_dto`::`ApplicationStatusDto`; _mediaType=nothing) -> `JobApplication`, `OpenAPI.Clients.ApiResponse` <br/>
> `update_job_application_status`(_api::`JobApplicationApi`, response_stream::`Channel`, `application_id`::`String`, `application_status_dto`::`ApplicationStatusDto`; _mediaType=nothing) -> `Channel`{ `JobApplication` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`JobApplicationApi`** | API context | 
**`application_id`** | **`String`** |  |
**`application_status_dto`** | [**`ApplicationStatusDto`**](ApplicationStatusDto.md) |  |

### Return type

[**`JobApplication`**](JobApplication.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

