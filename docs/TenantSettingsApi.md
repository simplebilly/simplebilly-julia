# TenantSettingsApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_tenant_settings**](TenantSettingsApi.md#get_tenant_settings) | **GET** /api/v1/settings/tenant | 
[**update_tenant_settings**](TenantSettingsApi.md#update_tenant_settings) | **PUT** /api/v1/settings/tenant | 


# **get_tenant_settings**
> `get_tenant_settings`(_api::`TenantSettingsApi`; _mediaType=nothing) -> `TenantSettings`, `OpenAPI.Clients.ApiResponse` <br/>
> `get_tenant_settings`(_api::`TenantSettingsApi`, response_stream::`Channel`; _mediaType=nothing) -> `Channel`{ `TenantSettings` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters
This endpoint does not need any parameter.

### Return type

[**`TenantSettings`**](TenantSettings.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **update_tenant_settings**
> `update_tenant_settings`(_api::`TenantSettingsApi`, `update_tenant_settings_param`::`UpdateTenantSettings`; _mediaType=nothing) -> `TenantSettings`, `OpenAPI.Clients.ApiResponse` <br/>
> `update_tenant_settings`(_api::`TenantSettingsApi`, response_stream::`Channel`, `update_tenant_settings_param`::`UpdateTenantSettings`; _mediaType=nothing) -> `Channel`{ `TenantSettings` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`TenantSettingsApi`** | API context | 
**`update_tenant_settings_param`** | [**`UpdateTenantSettings`**](UpdateTenantSettings.md) |  |

### Return type

[**`TenantSettings`**](TenantSettings.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

