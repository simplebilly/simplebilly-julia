# UserManagementApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_user**](UserManagementApi.md#get_user) | **GET** /api/v1/users/{user_id} | 
[**list_users**](UserManagementApi.md#list_users) | **GET** /api/v1/users | 
[**remove_user**](UserManagementApi.md#remove_user) | **DELETE** /api/v1/users/{user_id} | 
[**update_user_permissions**](UserManagementApi.md#update_user_permissions) | **PUT** /api/v1/users/{user_id}/permissions | 
[**update_user_role**](UserManagementApi.md#update_user_role) | **PUT** /api/v1/users/{user_id}/role | 


# **get_user**
> `get_user`(_api::`UserManagementApi`, `user_id`::`String`; _mediaType=nothing) -> `TenantUser`, `OpenAPI.Clients.ApiResponse` <br/>
> `get_user`(_api::`UserManagementApi`, response_stream::`Channel`, `user_id`::`String`; _mediaType=nothing) -> `Channel`{ `TenantUser` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`UserManagementApi`** | API context | 
**`user_id`** | **`String`** |  |

### Return type

[**`TenantUser`**](TenantUser.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **list_users**
> `list_users`(_api::`UserManagementApi`; _mediaType=nothing) -> `Vector{TenantUser}`, `OpenAPI.Clients.ApiResponse` <br/>
> `list_users`(_api::`UserManagementApi`, response_stream::`Channel`; _mediaType=nothing) -> `Channel`{ `Vector{TenantUser}` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters
This endpoint does not need any parameter.

### Return type

[**`Vector{TenantUser}`**](TenantUser.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **remove_user**
> `remove_user`(_api::`UserManagementApi`, `user_id`::`String`; _mediaType=nothing) -> `Nothing`, `OpenAPI.Clients.ApiResponse` <br/>
> `remove_user`(_api::`UserManagementApi`, response_stream::`Channel`, `user_id`::`String`; _mediaType=nothing) -> `Channel`{ `Nothing` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`UserManagementApi`** | API context | 
**`user_id`** | **`String`** |  |

### Return type

`Nothing`

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **update_user_permissions**
> `update_user_permissions`(_api::`UserManagementApi`, `user_id`::`String`, `update_permissions_payload`::`UpdatePermissionsPayload`; _mediaType=nothing) -> `Nothing`, `OpenAPI.Clients.ApiResponse` <br/>
> `update_user_permissions`(_api::`UserManagementApi`, response_stream::`Channel`, `user_id`::`String`, `update_permissions_payload`::`UpdatePermissionsPayload`; _mediaType=nothing) -> `Channel`{ `Nothing` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`UserManagementApi`** | API context | 
**`user_id`** | **`String`** |  |
**`update_permissions_payload`** | [**`UpdatePermissionsPayload`**](UpdatePermissionsPayload.md) |  |

### Return type

`Nothing`

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **update_user_role**
> `update_user_role`(_api::`UserManagementApi`, `user_id`::`String`, `update_role_payload`::`UpdateRolePayload`; _mediaType=nothing) -> `Nothing`, `OpenAPI.Clients.ApiResponse` <br/>
> `update_user_role`(_api::`UserManagementApi`, response_stream::`Channel`, `user_id`::`String`, `update_role_payload`::`UpdateRolePayload`; _mediaType=nothing) -> `Channel`{ `Nothing` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`UserManagementApi`** | API context | 
**`user_id`** | **`String`** |  |
**`update_role_payload`** | [**`UpdateRolePayload`**](UpdateRolePayload.md) |  |

### Return type

`Nothing`

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

