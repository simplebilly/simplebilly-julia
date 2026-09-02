# EmailTemplateApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_email_template**](EmailTemplateApi.md#create_email_template) | **POST** /api/v1/email-templates | 
[**delete_email_template**](EmailTemplateApi.md#delete_email_template) | **DELETE** /api/v1/email-templates/{email_template_id} | 
[**get_email_template**](EmailTemplateApi.md#get_email_template) | **GET** /api/v1/email-templates/{email_template_id} | 
[**list_email_templates**](EmailTemplateApi.md#list_email_templates) | **GET** /api/v1/email-templates/ | 
[**render_email_template**](EmailTemplateApi.md#render_email_template) | **POST** /api/v1/email-templates/{email_template_id}/render | 
[**update_email_template**](EmailTemplateApi.md#update_email_template) | **PUT** /api/v1/email-templates/{email_template_id} | 


# **create_email_template**
> `create_email_template`(_api::`EmailTemplateApi`, `email_template_create`::`EmailTemplateCreate`; _mediaType=nothing) -> `EmailTemplate`, `OpenAPI.Clients.ApiResponse` <br/>
> `create_email_template`(_api::`EmailTemplateApi`, response_stream::`Channel`, `email_template_create`::`EmailTemplateCreate`; _mediaType=nothing) -> `Channel`{ `EmailTemplate` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`EmailTemplateApi`** | API context | 
**`email_template_create`** | [**`EmailTemplateCreate`**](EmailTemplateCreate.md) |  |

### Return type

[**`EmailTemplate`**](EmailTemplate.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **delete_email_template**
> `delete_email_template`(_api::`EmailTemplateApi`, `email_template_id`::`String`; _mediaType=nothing) -> `Nothing`, `OpenAPI.Clients.ApiResponse` <br/>
> `delete_email_template`(_api::`EmailTemplateApi`, response_stream::`Channel`, `email_template_id`::`String`; _mediaType=nothing) -> `Channel`{ `Nothing` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`EmailTemplateApi`** | API context | 
**`email_template_id`** | **`String`** |  |

### Return type

`Nothing`

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **get_email_template**
> `get_email_template`(_api::`EmailTemplateApi`, `email_template_id`::`String`; _mediaType=nothing) -> `EmailTemplate`, `OpenAPI.Clients.ApiResponse` <br/>
> `get_email_template`(_api::`EmailTemplateApi`, response_stream::`Channel`, `email_template_id`::`String`; _mediaType=nothing) -> `Channel`{ `EmailTemplate` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`EmailTemplateApi`** | API context | 
**`email_template_id`** | **`String`** |  |

### Return type

[**`EmailTemplate`**](EmailTemplate.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **list_email_templates**
> `list_email_templates`(_api::`EmailTemplateApi`; `page`=nothing, `page_size`=nothing, `status`=nothing, `search`=nothing, _mediaType=nothing) -> `Vector{EmailTemplate}`, `OpenAPI.Clients.ApiResponse` <br/>
> `list_email_templates`(_api::`EmailTemplateApi`, response_stream::`Channel`; `page`=nothing, `page_size`=nothing, `status`=nothing, `search`=nothing, _mediaType=nothing) -> `Channel`{ `Vector{EmailTemplate}` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`EmailTemplateApi`** | API context | 

### Optional Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **`page`** | **`Int64`** |  | [default to nothing]
 **`page_size`** | **`Int64`** |  | [default to nothing]
 **`status`** | **`String`** |  | [default to nothing]
 **`search`** | **`String`** |  | [default to nothing]

### Return type

[**`Vector{EmailTemplate}`**](EmailTemplate.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **render_email_template**
> `render_email_template`(_api::`EmailTemplateApi`, `email_template_id`::`String`, `body`::`Any`; _mediaType=nothing) -> `Any`, `OpenAPI.Clients.ApiResponse` <br/>
> `render_email_template`(_api::`EmailTemplateApi`, response_stream::`Channel`, `email_template_id`::`String`, `body`::`Any`; _mediaType=nothing) -> `Channel`{ `Any` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`EmailTemplateApi`** | API context | 
**`email_template_id`** | **`String`** |  |
**`body`** | **`Any`** |  |

### Return type

**`Any`**

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **update_email_template**
> `update_email_template`(_api::`EmailTemplateApi`, `email_template_id`::`String`, `email_template_update`::`EmailTemplateUpdate`; _mediaType=nothing) -> `EmailTemplate`, `OpenAPI.Clients.ApiResponse` <br/>
> `update_email_template`(_api::`EmailTemplateApi`, response_stream::`Channel`, `email_template_id`::`String`, `email_template_update`::`EmailTemplateUpdate`; _mediaType=nothing) -> `Channel`{ `EmailTemplate` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`EmailTemplateApi`** | API context | 
**`email_template_id`** | **`String`** |  |
**`email_template_update`** | [**`EmailTemplateUpdate`**](EmailTemplateUpdate.md) |  |

### Return type

[**`EmailTemplate`**](EmailTemplate.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

