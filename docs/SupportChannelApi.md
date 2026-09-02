# SupportChannelApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_channel_api**](SupportChannelApi.md#create_channel_api) | **POST** /api/v1/support/channels | 
[**delete_channel_api**](SupportChannelApi.md#delete_channel_api) | **DELETE** /api/v1/support/channels/{channel_id} | 
[**list_channels_api**](SupportChannelApi.md#list_channels_api) | **GET** /api/v1/support/channels | 
[**update_channel_api**](SupportChannelApi.md#update_channel_api) | **PUT** /api/v1/support/channels/{channel_id} | 


# **create_channel_api**
> `create_channel_api`(_api::`SupportChannelApi`, `create_channel_dto`::`CreateChannelDto`; _mediaType=nothing) -> `SupportChannel`, `OpenAPI.Clients.ApiResponse` <br/>
> `create_channel_api`(_api::`SupportChannelApi`, response_stream::`Channel`, `create_channel_dto`::`CreateChannelDto`; _mediaType=nothing) -> `Channel`{ `SupportChannel` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`SupportChannelApi`** | API context | 
**`create_channel_dto`** | [**`CreateChannelDto`**](CreateChannelDto.md) |  |

### Return type

[**`SupportChannel`**](SupportChannel.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **delete_channel_api**
> `delete_channel_api`(_api::`SupportChannelApi`, `channel_id`::`String`; _mediaType=nothing) -> `Nothing`, `OpenAPI.Clients.ApiResponse` <br/>
> `delete_channel_api`(_api::`SupportChannelApi`, response_stream::`Channel`, `channel_id`::`String`; _mediaType=nothing) -> `Channel`{ `Nothing` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`SupportChannelApi`** | API context | 
**`channel_id`** | **`String`** |  |

### Return type

`Nothing`

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **list_channels_api**
> `list_channels_api`(_api::`SupportChannelApi`; _mediaType=nothing) -> `Vector{SupportChannel}`, `OpenAPI.Clients.ApiResponse` <br/>
> `list_channels_api`(_api::`SupportChannelApi`, response_stream::`Channel`; _mediaType=nothing) -> `Channel`{ `Vector{SupportChannel}` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters
This endpoint does not need any parameter.

### Return type

[**`Vector{SupportChannel}`**](SupportChannel.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **update_channel_api**
> `update_channel_api`(_api::`SupportChannelApi`, `channel_id`::`String`, `update_channel_dto`::`UpdateChannelDto`; _mediaType=nothing) -> `SupportChannel`, `OpenAPI.Clients.ApiResponse` <br/>
> `update_channel_api`(_api::`SupportChannelApi`, response_stream::`Channel`, `channel_id`::`String`, `update_channel_dto`::`UpdateChannelDto`; _mediaType=nothing) -> `Channel`{ `SupportChannel` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`SupportChannelApi`** | API context | 
**`channel_id`** | **`String`** |  |
**`update_channel_dto`** | [**`UpdateChannelDto`**](UpdateChannelDto.md) |  |

### Return type

[**`SupportChannel`**](SupportChannel.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

