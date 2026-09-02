# MarketplaceApiApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_connection_api**](MarketplaceApiApi.md#create_connection_api) | **POST** /api/v1/marketplace/connections | Create a new connection (for API-key based platforms)
[**delete_connection_api**](MarketplaceApiApi.md#delete_connection_api) | **DELETE** /api/v1/marketplace/connections/{connection_id} | Soft-delete a connection
[**get_connection_api**](MarketplaceApiApi.md#get_connection_api) | **GET** /api/v1/marketplace/connections/{connection_id} | Get a single connection
[**get_sync_direction_api**](MarketplaceApiApi.md#get_sync_direction_api) | **GET** /api/v1/marketplace/connections/{connection_id}/directions | Get current sync direction configuration for a connection
[**get_sync_logs_api**](MarketplaceApiApi.md#get_sync_logs_api) | **GET** /api/v1/marketplace/connections/{connection_id}/logs | Get sync logs for a connection
[**list_connections_api**](MarketplaceApiApi.md#list_connections_api) | **GET** /api/v1/marketplace/connections | List connections for the current tenant
[**list_platforms_api**](MarketplaceApiApi.md#list_platforms_api) | **GET** /api/v1/marketplace/platforms | List all supported platforms
[**oauth_authorize_api**](MarketplaceApiApi.md#oauth_authorize_api) | **POST** /api/v1/marketplace/oauth/authorize | OAuth: initiate authorization flow
[**oauth_callback_api**](MarketplaceApiApi.md#oauth_callback_api) | **POST** /api/v1/marketplace/oauth/callback | OAuth: handle callback after authorization
[**trigger_sync_api**](MarketplaceApiApi.md#trigger_sync_api) | **POST** /api/v1/marketplace/connections/{connection_id}/sync | Trigger sync for a connection
[**update_connection_api**](MarketplaceApiApi.md#update_connection_api) | **PUT** /api/v1/marketplace/connections/{connection_id} | Update a connection
[**update_sync_direction_api**](MarketplaceApiApi.md#update_sync_direction_api) | **PUT** /api/v1/marketplace/connections/{connection_id}/directions | Update per-entity sync direction configuration for a connection
[**webhook_receiver_api**](MarketplaceApiApi.md#webhook_receiver_api) | **POST** /api/v1/marketplace/webhook/{platform}/{connection_id} | Webhook receiver


# **create_connection_api**
> `create_connection_api`(_api::`MarketplaceApiApi`, `create_connection_request`::`CreateConnectionRequest`; _mediaType=nothing) -> `MarketplaceConnection`, `OpenAPI.Clients.ApiResponse` <br/>
> `create_connection_api`(_api::`MarketplaceApiApi`, response_stream::`Channel`, `create_connection_request`::`CreateConnectionRequest`; _mediaType=nothing) -> `Channel`{ `MarketplaceConnection` }, `OpenAPI.Clients.ApiResponse`

Create a new connection (for API-key based platforms)

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`MarketplaceApiApi`** | API context | 
**`create_connection_request`** | [**`CreateConnectionRequest`**](CreateConnectionRequest.md) |  |

### Return type

[**`MarketplaceConnection`**](MarketplaceConnection.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **delete_connection_api**
> `delete_connection_api`(_api::`MarketplaceApiApi`, `connection_id`::`String`; _mediaType=nothing) -> `Nothing`, `OpenAPI.Clients.ApiResponse` <br/>
> `delete_connection_api`(_api::`MarketplaceApiApi`, response_stream::`Channel`, `connection_id`::`String`; _mediaType=nothing) -> `Channel`{ `Nothing` }, `OpenAPI.Clients.ApiResponse`

Soft-delete a connection

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`MarketplaceApiApi`** | API context | 
**`connection_id`** | **`String`** |  |

### Return type

`Nothing`

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **get_connection_api**
> `get_connection_api`(_api::`MarketplaceApiApi`, `connection_id`::`String`; _mediaType=nothing) -> `MarketplaceConnection`, `OpenAPI.Clients.ApiResponse` <br/>
> `get_connection_api`(_api::`MarketplaceApiApi`, response_stream::`Channel`, `connection_id`::`String`; _mediaType=nothing) -> `Channel`{ `MarketplaceConnection` }, `OpenAPI.Clients.ApiResponse`

Get a single connection

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`MarketplaceApiApi`** | API context | 
**`connection_id`** | **`String`** |  |

### Return type

[**`MarketplaceConnection`**](MarketplaceConnection.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **get_sync_direction_api**
> `get_sync_direction_api`(_api::`MarketplaceApiApi`, `connection_id`::`String`; _mediaType=nothing) -> `Nothing`, `OpenAPI.Clients.ApiResponse` <br/>
> `get_sync_direction_api`(_api::`MarketplaceApiApi`, response_stream::`Channel`, `connection_id`::`String`; _mediaType=nothing) -> `Channel`{ `Nothing` }, `OpenAPI.Clients.ApiResponse`

Get current sync direction configuration for a connection

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`MarketplaceApiApi`** | API context | 
**`connection_id`** | **`String`** |  |

### Return type

`Nothing`

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **get_sync_logs_api**
> `get_sync_logs_api`(_api::`MarketplaceApiApi`, `connection_id`::`String`; _mediaType=nothing) -> `Vector{SyncLog}`, `OpenAPI.Clients.ApiResponse` <br/>
> `get_sync_logs_api`(_api::`MarketplaceApiApi`, response_stream::`Channel`, `connection_id`::`String`; _mediaType=nothing) -> `Channel`{ `Vector{SyncLog}` }, `OpenAPI.Clients.ApiResponse`

Get sync logs for a connection

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`MarketplaceApiApi`** | API context | 
**`connection_id`** | **`String`** |  |

### Return type

[**`Vector{SyncLog}`**](SyncLog.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **list_connections_api**
> `list_connections_api`(_api::`MarketplaceApiApi`; _mediaType=nothing) -> `Vector{MarketplaceConnection}`, `OpenAPI.Clients.ApiResponse` <br/>
> `list_connections_api`(_api::`MarketplaceApiApi`, response_stream::`Channel`; _mediaType=nothing) -> `Channel`{ `Vector{MarketplaceConnection}` }, `OpenAPI.Clients.ApiResponse`

List connections for the current tenant

### Required Parameters
This endpoint does not need any parameter.

### Return type

[**`Vector{MarketplaceConnection}`**](MarketplaceConnection.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **list_platforms_api**
> `list_platforms_api`(_api::`MarketplaceApiApi`; _mediaType=nothing) -> `Vector{PlatformInfo}`, `OpenAPI.Clients.ApiResponse` <br/>
> `list_platforms_api`(_api::`MarketplaceApiApi`, response_stream::`Channel`; _mediaType=nothing) -> `Channel`{ `Vector{PlatformInfo}` }, `OpenAPI.Clients.ApiResponse`

List all supported platforms

### Required Parameters
This endpoint does not need any parameter.

### Return type

[**`Vector{PlatformInfo}`**](PlatformInfo.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **oauth_authorize_api**
> `oauth_authorize_api`(_api::`MarketplaceApiApi`, `o_auth_authorize_request`::`OAuthAuthorizeRequest`; _mediaType=nothing) -> `OAuthAuthorizeResponse`, `OpenAPI.Clients.ApiResponse` <br/>
> `oauth_authorize_api`(_api::`MarketplaceApiApi`, response_stream::`Channel`, `o_auth_authorize_request`::`OAuthAuthorizeRequest`; _mediaType=nothing) -> `Channel`{ `OAuthAuthorizeResponse` }, `OpenAPI.Clients.ApiResponse`

OAuth: initiate authorization flow

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`MarketplaceApiApi`** | API context | 
**`o_auth_authorize_request`** | [**`OAuthAuthorizeRequest`**](OAuthAuthorizeRequest.md) |  |

### Return type

[**`OAuthAuthorizeResponse`**](OAuthAuthorizeResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **oauth_callback_api**
> `oauth_callback_api`(_api::`MarketplaceApiApi`, `o_auth_callback_request`::`OAuthCallbackRequest`; _mediaType=nothing) -> `MarketplaceConnection`, `OpenAPI.Clients.ApiResponse` <br/>
> `oauth_callback_api`(_api::`MarketplaceApiApi`, response_stream::`Channel`, `o_auth_callback_request`::`OAuthCallbackRequest`; _mediaType=nothing) -> `Channel`{ `MarketplaceConnection` }, `OpenAPI.Clients.ApiResponse`

OAuth: handle callback after authorization

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`MarketplaceApiApi`** | API context | 
**`o_auth_callback_request`** | [**`OAuthCallbackRequest`**](OAuthCallbackRequest.md) |  |

### Return type

[**`MarketplaceConnection`**](MarketplaceConnection.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **trigger_sync_api**
> `trigger_sync_api`(_api::`MarketplaceApiApi`, `connection_id`::`String`; `sync_type`=nothing, `direction`=nothing, _mediaType=nothing) -> `SyncSummary`, `OpenAPI.Clients.ApiResponse` <br/>
> `trigger_sync_api`(_api::`MarketplaceApiApi`, response_stream::`Channel`, `connection_id`::`String`; `sync_type`=nothing, `direction`=nothing, _mediaType=nothing) -> `Channel`{ `SyncSummary` }, `OpenAPI.Clients.ApiResponse`

Trigger sync for a connection

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`MarketplaceApiApi`** | API context | 
**`connection_id`** | **`String`** |  |

### Optional Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **`sync_type`** | **`String`** |  | [default to nothing]
 **`direction`** | **`String`** |  | [default to nothing]

### Return type

[**`SyncSummary`**](SyncSummary.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **update_connection_api**
> `update_connection_api`(_api::`MarketplaceApiApi`, `connection_id`::`String`, `update_connection_request`::`UpdateConnectionRequest`; _mediaType=nothing) -> `MarketplaceConnection`, `OpenAPI.Clients.ApiResponse` <br/>
> `update_connection_api`(_api::`MarketplaceApiApi`, response_stream::`Channel`, `connection_id`::`String`, `update_connection_request`::`UpdateConnectionRequest`; _mediaType=nothing) -> `Channel`{ `MarketplaceConnection` }, `OpenAPI.Clients.ApiResponse`

Update a connection

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`MarketplaceApiApi`** | API context | 
**`connection_id`** | **`String`** |  |
**`update_connection_request`** | [**`UpdateConnectionRequest`**](UpdateConnectionRequest.md) |  |

### Return type

[**`MarketplaceConnection`**](MarketplaceConnection.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **update_sync_direction_api**
> `update_sync_direction_api`(_api::`MarketplaceApiApi`, `connection_id`::`String`, `update_sync_direction_request`::`UpdateSyncDirectionRequest`; _mediaType=nothing) -> `Nothing`, `OpenAPI.Clients.ApiResponse` <br/>
> `update_sync_direction_api`(_api::`MarketplaceApiApi`, response_stream::`Channel`, `connection_id`::`String`, `update_sync_direction_request`::`UpdateSyncDirectionRequest`; _mediaType=nothing) -> `Channel`{ `Nothing` }, `OpenAPI.Clients.ApiResponse`

Update per-entity sync direction configuration for a connection

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`MarketplaceApiApi`** | API context | 
**`connection_id`** | **`String`** |  |
**`update_sync_direction_request`** | [**`UpdateSyncDirectionRequest`**](UpdateSyncDirectionRequest.md) |  |

### Return type

`Nothing`

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **webhook_receiver_api**
> `webhook_receiver_api`(_api::`MarketplaceApiApi`, `platform`::`String`, `connection_id`::`String`; _mediaType=nothing) -> `Nothing`, `OpenAPI.Clients.ApiResponse` <br/>
> `webhook_receiver_api`(_api::`MarketplaceApiApi`, response_stream::`Channel`, `platform`::`String`, `connection_id`::`String`; _mediaType=nothing) -> `Channel`{ `Nothing` }, `OpenAPI.Clients.ApiResponse`

Webhook receiver

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`MarketplaceApiApi`** | API context | 
**`platform`** | **`String`** |  |
**`connection_id`** | **`String`** |  |

### Return type

`Nothing`

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

