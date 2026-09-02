# AutomationsApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**list_automations**](AutomationsApi.md#list_automations) | **GET** /api/v1/automations | 
[**trigger_automation**](AutomationsApi.md#trigger_automation) | **POST** /api/v1/automations/{key}/trigger | 
[**update_automation**](AutomationsApi.md#update_automation) | **PUT** /api/v1/automations/{key} | 


# **list_automations**
> `list_automations`(_api::`AutomationsApi`; _mediaType=nothing) -> `Vector{AutomationDto}`, `OpenAPI.Clients.ApiResponse` <br/>
> `list_automations`(_api::`AutomationsApi`, response_stream::`Channel`; _mediaType=nothing) -> `Channel`{ `Vector{AutomationDto}` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters
This endpoint does not need any parameter.

### Return type

[**`Vector{AutomationDto}`**](AutomationDto.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **trigger_automation**
> `trigger_automation`(_api::`AutomationsApi`, `key`::`String`; _mediaType=nothing) -> `Any`, `OpenAPI.Clients.ApiResponse` <br/>
> `trigger_automation`(_api::`AutomationsApi`, response_stream::`Channel`, `key`::`String`; _mediaType=nothing) -> `Channel`{ `Any` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`AutomationsApi`** | API context | 
**`key`** | **`String`** |  |

### Return type

**`Any`**

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **update_automation**
> `update_automation`(_api::`AutomationsApi`, `key`::`String`, `update_automation_param`::`UpdateAutomation`; _mediaType=nothing) -> `AutomationDto`, `OpenAPI.Clients.ApiResponse` <br/>
> `update_automation`(_api::`AutomationsApi`, response_stream::`Channel`, `key`::`String`, `update_automation_param`::`UpdateAutomation`; _mediaType=nothing) -> `Channel`{ `AutomationDto` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`AutomationsApi`** | API context | 
**`key`** | **`String`** |  |
**`update_automation_param`** | [**`UpdateAutomation`**](UpdateAutomation.md) |  |

### Return type

[**`AutomationDto`**](AutomationDto.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

