# LeadApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**list_leads_api**](LeadApi.md#list_leads_api) | **GET** /api/v1/support/leads | 
[**update_lead_api**](LeadApi.md#update_lead_api) | **PUT** /api/v1/support/leads/{lead_id} | 


# **list_leads_api**
> `list_leads_api`(_api::`LeadApi`; `status`=nothing, `source`=nothing, `search`=nothing, `page`=nothing, `page_size`=nothing, _mediaType=nothing) -> `Vector{Lead}`, `OpenAPI.Clients.ApiResponse` <br/>
> `list_leads_api`(_api::`LeadApi`, response_stream::`Channel`; `status`=nothing, `source`=nothing, `search`=nothing, `page`=nothing, `page_size`=nothing, _mediaType=nothing) -> `Channel`{ `Vector{Lead}` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`LeadApi`** | API context | 

### Optional Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **`status`** | **`String`** |  | [default to nothing]
 **`source`** | **`String`** |  | [default to nothing]
 **`search`** | **`String`** |  | [default to nothing]
 **`page`** | **`Int64`** |  | [default to nothing]
 **`page_size`** | **`Int64`** |  | [default to nothing]

### Return type

[**`Vector{Lead}`**](Lead.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **update_lead_api**
> `update_lead_api`(_api::`LeadApi`, `lead_id`::`String`, `lead_update`::`LeadUpdate`; _mediaType=nothing) -> `Lead`, `OpenAPI.Clients.ApiResponse` <br/>
> `update_lead_api`(_api::`LeadApi`, response_stream::`Channel`, `lead_id`::`String`, `lead_update`::`LeadUpdate`; _mediaType=nothing) -> `Channel`{ `Lead` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`LeadApi`** | API context | 
**`lead_id`** | **`String`** |  |
**`lead_update`** | [**`LeadUpdate`**](LeadUpdate.md) |  |

### Return type

[**`Lead`**](Lead.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

