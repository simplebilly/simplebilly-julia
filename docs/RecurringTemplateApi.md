# RecurringTemplateApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_recurring_template**](RecurringTemplateApi.md#create_recurring_template) | **POST** /api/v1/recurring-templates | 
[**delete_recurring_template**](RecurringTemplateApi.md#delete_recurring_template) | **DELETE** /api/v1/recurring-templates/{template_id} | 
[**get_recurring_template**](RecurringTemplateApi.md#get_recurring_template) | **GET** /api/v1/recurring-templates/{template_id} | 
[**list_recurring_templates**](RecurringTemplateApi.md#list_recurring_templates) | **GET** /api/v1/recurring-templates/ | 


# **create_recurring_template**
> `create_recurring_template`(_api::`RecurringTemplateApi`, `body`::`Any`; _mediaType=nothing) -> `RecurringTemplate`, `OpenAPI.Clients.ApiResponse` <br/>
> `create_recurring_template`(_api::`RecurringTemplateApi`, response_stream::`Channel`, `body`::`Any`; _mediaType=nothing) -> `Channel`{ `RecurringTemplate` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`RecurringTemplateApi`** | API context | 
**`body`** | **`Any`** |  |

### Return type

[**`RecurringTemplate`**](RecurringTemplate.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **delete_recurring_template**
> `delete_recurring_template`(_api::`RecurringTemplateApi`, `template_id`::`String`; _mediaType=nothing) -> `Nothing`, `OpenAPI.Clients.ApiResponse` <br/>
> `delete_recurring_template`(_api::`RecurringTemplateApi`, response_stream::`Channel`, `template_id`::`String`; _mediaType=nothing) -> `Channel`{ `Nothing` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`RecurringTemplateApi`** | API context | 
**`template_id`** | **`String`** |  |

### Return type

`Nothing`

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **get_recurring_template**
> `get_recurring_template`(_api::`RecurringTemplateApi`, `template_id`::`String`; _mediaType=nothing) -> `RecurringTemplate`, `OpenAPI.Clients.ApiResponse` <br/>
> `get_recurring_template`(_api::`RecurringTemplateApi`, response_stream::`Channel`, `template_id`::`String`; _mediaType=nothing) -> `Channel`{ `RecurringTemplate` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`RecurringTemplateApi`** | API context | 
**`template_id`** | **`String`** |  |

### Return type

[**`RecurringTemplate`**](RecurringTemplate.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **list_recurring_templates**
> `list_recurring_templates`(_api::`RecurringTemplateApi`; _mediaType=nothing) -> `Vector{RecurringTemplate}`, `OpenAPI.Clients.ApiResponse` <br/>
> `list_recurring_templates`(_api::`RecurringTemplateApi`, response_stream::`Channel`; _mediaType=nothing) -> `Channel`{ `Vector{RecurringTemplate}` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters
This endpoint does not need any parameter.

### Return type

[**`Vector{RecurringTemplate}`**](RecurringTemplate.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

