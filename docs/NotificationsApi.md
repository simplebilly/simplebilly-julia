# NotificationsApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**delete_notification**](NotificationsApi.md#delete_notification) | **DELETE** /api/v1/notifications/{id} | 
[**list_notifications**](NotificationsApi.md#list_notifications) | **GET** /api/v1/notifications | 
[**mark_all_read**](NotificationsApi.md#mark_all_read) | **PUT** /api/v1/notifications/read-all | 
[**mark_as_read**](NotificationsApi.md#mark_as_read) | **PUT** /api/v1/notifications/{id}/read | 
[**unread_count**](NotificationsApi.md#unread_count) | **GET** /api/v1/notifications/unread-count | 


# **delete_notification**
> `delete_notification`(_api::`NotificationsApi`, `id`::`String`; _mediaType=nothing) -> `Nothing`, `OpenAPI.Clients.ApiResponse` <br/>
> `delete_notification`(_api::`NotificationsApi`, response_stream::`Channel`, `id`::`String`; _mediaType=nothing) -> `Channel`{ `Nothing` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`NotificationsApi`** | API context | 
**`id`** | **`String`** |  |

### Return type

`Nothing`

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **list_notifications**
> `list_notifications`(_api::`NotificationsApi`; _mediaType=nothing) -> `Vector{NotificationDto}`, `OpenAPI.Clients.ApiResponse` <br/>
> `list_notifications`(_api::`NotificationsApi`, response_stream::`Channel`; _mediaType=nothing) -> `Channel`{ `Vector{NotificationDto}` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters
This endpoint does not need any parameter.

### Return type

[**`Vector{NotificationDto}`**](NotificationDto.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **mark_all_read**
> `mark_all_read`(_api::`NotificationsApi`; _mediaType=nothing) -> `Int64`, `OpenAPI.Clients.ApiResponse` <br/>
> `mark_all_read`(_api::`NotificationsApi`, response_stream::`Channel`; _mediaType=nothing) -> `Channel`{ `Int64` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters
This endpoint does not need any parameter.

### Return type

**`Int64`**

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: text/plain

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **mark_as_read**
> `mark_as_read`(_api::`NotificationsApi`, `id`::`String`; _mediaType=nothing) -> `Nothing`, `OpenAPI.Clients.ApiResponse` <br/>
> `mark_as_read`(_api::`NotificationsApi`, response_stream::`Channel`, `id`::`String`; _mediaType=nothing) -> `Channel`{ `Nothing` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`NotificationsApi`** | API context | 
**`id`** | **`String`** |  |

### Return type

`Nothing`

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **unread_count**
> `unread_count`(_api::`NotificationsApi`; _mediaType=nothing) -> `Int64`, `OpenAPI.Clients.ApiResponse` <br/>
> `unread_count`(_api::`NotificationsApi`, response_stream::`Channel`; _mediaType=nothing) -> `Channel`{ `Int64` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters
This endpoint does not need any parameter.

### Return type

**`Int64`**

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: text/plain

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

