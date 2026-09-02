# ActivityApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_activity**](ActivityApi.md#create_activity) | **POST** /api/v1/activities | 
[**delete_activity**](ActivityApi.md#delete_activity) | **DELETE** /api/v1/activities/{activity_id} | 
[**get_activity**](ActivityApi.md#get_activity) | **GET** /api/v1/activities/{activity_id} | 
[**list_activities**](ActivityApi.md#list_activities) | **GET** /api/v1/activities/ | 
[**update_activity**](ActivityApi.md#update_activity) | **PUT** /api/v1/activities/{activity_id} | 
[**update_activity_status**](ActivityApi.md#update_activity_status) | **PUT** /api/v1/activities/{activity_id}/status | 


# **create_activity**
> `create_activity`(_api::`ActivityApi`, `activity`::`Activity`; _mediaType=nothing) -> `Activity`, `OpenAPI.Clients.ApiResponse` <br/>
> `create_activity`(_api::`ActivityApi`, response_stream::`Channel`, `activity`::`Activity`; _mediaType=nothing) -> `Channel`{ `Activity` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ActivityApi`** | API context | 
**`activity`** | [**`Activity`**](Activity.md) |  |

### Return type

[**`Activity`**](Activity.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **delete_activity**
> `delete_activity`(_api::`ActivityApi`, `activity_id`::`String`; _mediaType=nothing) -> `Nothing`, `OpenAPI.Clients.ApiResponse` <br/>
> `delete_activity`(_api::`ActivityApi`, response_stream::`Channel`, `activity_id`::`String`; _mediaType=nothing) -> `Channel`{ `Nothing` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ActivityApi`** | API context | 
**`activity_id`** | **`String`** |  |

### Return type

`Nothing`

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **get_activity**
> `get_activity`(_api::`ActivityApi`, `activity_id`::`String`; _mediaType=nothing) -> `Activity`, `OpenAPI.Clients.ApiResponse` <br/>
> `get_activity`(_api::`ActivityApi`, response_stream::`Channel`, `activity_id`::`String`; _mediaType=nothing) -> `Channel`{ `Activity` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ActivityApi`** | API context | 
**`activity_id`** | **`String`** |  |

### Return type

[**`Activity`**](Activity.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **list_activities**
> `list_activities`(_api::`ActivityApi`; `page`=nothing, `page_size`=nothing, `contact_id`=nothing, `activity_type`=nothing, `status`=nothing, `assigned_to`=nothing, `overdue_only`=nothing, _mediaType=nothing) -> `Vector{Activity}`, `OpenAPI.Clients.ApiResponse` <br/>
> `list_activities`(_api::`ActivityApi`, response_stream::`Channel`; `page`=nothing, `page_size`=nothing, `contact_id`=nothing, `activity_type`=nothing, `status`=nothing, `assigned_to`=nothing, `overdue_only`=nothing, _mediaType=nothing) -> `Channel`{ `Vector{Activity}` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ActivityApi`** | API context | 

### Optional Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **`page`** | **`Int64`** |  | [default to nothing]
 **`page_size`** | **`Int64`** |  | [default to nothing]
 **`contact_id`** | **`String`** |  | [default to nothing]
 **`activity_type`** | **`String`** |  | [default to nothing]
 **`status`** | **`String`** |  | [default to nothing]
 **`assigned_to`** | **`String`** |  | [default to nothing]
 **`overdue_only`** | **`Bool`** | Only show overdue follow-ups. | [default to nothing]

### Return type

[**`Vector{Activity}`**](Activity.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **update_activity**
> `update_activity`(_api::`ActivityApi`, `activity_id`::`String`, `body`::`Any`; _mediaType=nothing) -> `Activity`, `OpenAPI.Clients.ApiResponse` <br/>
> `update_activity`(_api::`ActivityApi`, response_stream::`Channel`, `activity_id`::`String`, `body`::`Any`; _mediaType=nothing) -> `Channel`{ `Activity` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ActivityApi`** | API context | 
**`activity_id`** | **`String`** |  |
**`body`** | **`Any`** |  |

### Return type

[**`Activity`**](Activity.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **update_activity_status**
> `update_activity_status`(_api::`ActivityApi`, `activity_id`::`String`, `activity_status_update`::`ActivityStatusUpdate`; _mediaType=nothing) -> `Activity`, `OpenAPI.Clients.ApiResponse` <br/>
> `update_activity_status`(_api::`ActivityApi`, response_stream::`Channel`, `activity_id`::`String`, `activity_status_update`::`ActivityStatusUpdate`; _mediaType=nothing) -> `Channel`{ `Activity` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ActivityApi`** | API context | 
**`activity_id`** | **`String`** |  |
**`activity_status_update`** | [**`ActivityStatusUpdate`**](ActivityStatusUpdate.md) |  |

### Return type

[**`Activity`**](Activity.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

