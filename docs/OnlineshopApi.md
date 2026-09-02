# OnlineshopApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_smtp_config_api**](OnlineshopApi.md#get_smtp_config_api) | **GET** /api/v1/settings/smtp | 
[**save_smtp_config_api**](OnlineshopApi.md#save_smtp_config_api) | **PUT** /api/v1/settings/smtp | 


# **get_smtp_config_api**
> `get_smtp_config_api`(_api::`OnlineshopApi`; _mediaType=nothing) -> `SmtpConfig`, `OpenAPI.Clients.ApiResponse` <br/>
> `get_smtp_config_api`(_api::`OnlineshopApi`, response_stream::`Channel`; _mediaType=nothing) -> `Channel`{ `SmtpConfig` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters
This endpoint does not need any parameter.

### Return type

[**`SmtpConfig`**](SmtpConfig.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **save_smtp_config_api**
> `save_smtp_config_api`(_api::`OnlineshopApi`; `smtp_config`=nothing, _mediaType=nothing) -> `SmtpConfig`, `OpenAPI.Clients.ApiResponse` <br/>
> `save_smtp_config_api`(_api::`OnlineshopApi`, response_stream::`Channel`; `smtp_config`=nothing, _mediaType=nothing) -> `Channel`{ `SmtpConfig` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`OnlineshopApi`** | API context | 

### Optional Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **`smtp_config`** | [**`SmtpConfig`**](SmtpConfig.md) |  | 

### Return type

[**`SmtpConfig`**](SmtpConfig.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

