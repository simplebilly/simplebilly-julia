# UserApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**change_password**](UserApi.md#change_password) | **POST** /user/change-password | Change the current user&#39;s password (requires the current password).
[**create_team**](UserApi.md#create_team) | **POST** /user/teams | Create a new team within the current tenant
[**generate_api_key**](UserApi.md#generate_api_key) | **POST** /user/api-key | Generate a new API key for the current user
[**invite_user**](UserApi.md#invite_user) | **POST** /user/invite | Invite a user to the current tenant/organization
[**list_teams**](UserApi.md#list_teams) | **GET** /user/teams | List all teams in the current tenant
[**remove_user_from_org**](UserApi.md#remove_user_from_org) | **DELETE** /user/remove | Remove a user from the current organization
[**update_profile**](UserApi.md#update_profile) | **PUT** /user/profile | Update the current user&#39;s profile
[**user_profile**](UserApi.md#user_profile) | **GET** /user/profile | Get the current user&#39;s profile
[**user_tenants**](UserApi.md#user_tenants) | **GET** /user/tenants | List all tenants (organizations) the current user belongs to


# **change_password**
> `change_password`(_api::`UserApi`, `change_password_request`::`ChangePasswordRequest`; _mediaType=nothing) -> `Nothing`, `OpenAPI.Clients.ApiResponse` <br/>
> `change_password`(_api::`UserApi`, response_stream::`Channel`, `change_password_request`::`ChangePasswordRequest`; _mediaType=nothing) -> `Channel`{ `Nothing` }, `OpenAPI.Clients.ApiResponse`

Change the current user's password (requires the current password).

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`UserApi`** | API context | 
**`change_password_request`** | [**`ChangePasswordRequest`**](ChangePasswordRequest.md) |  |

### Return type

`Nothing`

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **create_team**
> `create_team`(_api::`UserApi`, `team_create`::`TeamCreate`; _mediaType=nothing) -> `ApiResponseTeam`, `OpenAPI.Clients.ApiResponse` <br/>
> `create_team`(_api::`UserApi`, response_stream::`Channel`, `team_create`::`TeamCreate`; _mediaType=nothing) -> `Channel`{ `ApiResponseTeam` }, `OpenAPI.Clients.ApiResponse`

Create a new team within the current tenant

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`UserApi`** | API context | 
**`team_create`** | [**`TeamCreate`**](TeamCreate.md) |  |

### Return type

[**`ApiResponseTeam`**](ApiResponseTeam.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **generate_api_key**
> `generate_api_key`(_api::`UserApi`; _mediaType=nothing) -> `ApiResponseString`, `OpenAPI.Clients.ApiResponse` <br/>
> `generate_api_key`(_api::`UserApi`, response_stream::`Channel`; _mediaType=nothing) -> `Channel`{ `ApiResponseString` }, `OpenAPI.Clients.ApiResponse`

Generate a new API key for the current user

### Required Parameters
This endpoint does not need any parameter.

### Return type

[**`ApiResponseString`**](ApiResponseString.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **invite_user**
> `invite_user`(_api::`UserApi`, `invite_request`::`InviteRequest`; _mediaType=nothing) -> `Nothing`, `OpenAPI.Clients.ApiResponse` <br/>
> `invite_user`(_api::`UserApi`, response_stream::`Channel`, `invite_request`::`InviteRequest`; _mediaType=nothing) -> `Channel`{ `Nothing` }, `OpenAPI.Clients.ApiResponse`

Invite a user to the current tenant/organization

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`UserApi`** | API context | 
**`invite_request`** | [**`InviteRequest`**](InviteRequest.md) |  |

### Return type

`Nothing`

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **list_teams**
> `list_teams`(_api::`UserApi`; _mediaType=nothing) -> `ApiResponseVecTeam`, `OpenAPI.Clients.ApiResponse` <br/>
> `list_teams`(_api::`UserApi`, response_stream::`Channel`; _mediaType=nothing) -> `Channel`{ `ApiResponseVecTeam` }, `OpenAPI.Clients.ApiResponse`

List all teams in the current tenant

### Required Parameters
This endpoint does not need any parameter.

### Return type

[**`ApiResponseVecTeam`**](ApiResponseVecTeam.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **remove_user_from_org**
> `remove_user_from_org`(_api::`UserApi`, `remove_user_request`::`RemoveUserRequest`; _mediaType=nothing) -> `Nothing`, `OpenAPI.Clients.ApiResponse` <br/>
> `remove_user_from_org`(_api::`UserApi`, response_stream::`Channel`, `remove_user_request`::`RemoveUserRequest`; _mediaType=nothing) -> `Channel`{ `Nothing` }, `OpenAPI.Clients.ApiResponse`

Remove a user from the current organization

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`UserApi`** | API context | 
**`remove_user_request`** | [**`RemoveUserRequest`**](RemoveUserRequest.md) |  |

### Return type

`Nothing`

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **update_profile**
> `update_profile`(_api::`UserApi`, `update_profile_request`::`UpdateProfileRequest`; _mediaType=nothing) -> `Nothing`, `OpenAPI.Clients.ApiResponse` <br/>
> `update_profile`(_api::`UserApi`, response_stream::`Channel`, `update_profile_request`::`UpdateProfileRequest`; _mediaType=nothing) -> `Channel`{ `Nothing` }, `OpenAPI.Clients.ApiResponse`

Update the current user's profile

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`UserApi`** | API context | 
**`update_profile_request`** | [**`UpdateProfileRequest`**](UpdateProfileRequest.md) |  |

### Return type

`Nothing`

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **user_profile**
> `user_profile`(_api::`UserApi`; _mediaType=nothing) -> `ApiResponseUserProfile`, `OpenAPI.Clients.ApiResponse` <br/>
> `user_profile`(_api::`UserApi`, response_stream::`Channel`; _mediaType=nothing) -> `Channel`{ `ApiResponseUserProfile` }, `OpenAPI.Clients.ApiResponse`

Get the current user's profile

### Required Parameters
This endpoint does not need any parameter.

### Return type

[**`ApiResponseUserProfile`**](ApiResponseUserProfile.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **user_tenants**
> `user_tenants`(_api::`UserApi`; _mediaType=nothing) -> `ApiResponseVecUserTenantInfo`, `OpenAPI.Clients.ApiResponse` <br/>
> `user_tenants`(_api::`UserApi`, response_stream::`Channel`; _mediaType=nothing) -> `Channel`{ `ApiResponseVecUserTenantInfo` }, `OpenAPI.Clients.ApiResponse`

List all tenants (organizations) the current user belongs to

### Required Parameters
This endpoint does not need any parameter.

### Return type

[**`ApiResponseVecUserTenantInfo`**](ApiResponseVecUserTenantInfo.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

