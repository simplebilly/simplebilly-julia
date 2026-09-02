# WorkflowsApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**list_workflows_api**](WorkflowsApi.md#list_workflows_api) | **GET** /api/v1/workflows | 
[**set_workflow_enabled_api**](WorkflowsApi.md#set_workflow_enabled_api) | **PUT** /api/v1/workflows/{workflow_id}/enabled | 


# **list_workflows_api**
> `list_workflows_api`(_api::`WorkflowsApi`; _mediaType=nothing) -> `Vector{Workflow}`, `OpenAPI.Clients.ApiResponse` <br/>
> `list_workflows_api`(_api::`WorkflowsApi`, response_stream::`Channel`; _mediaType=nothing) -> `Channel`{ `Vector{Workflow}` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters
This endpoint does not need any parameter.

### Return type

[**`Vector{Workflow}`**](Workflow.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **set_workflow_enabled_api**
> `set_workflow_enabled_api`(_api::`WorkflowsApi`, `workflow_id`::`String`, `workflow_enabled_update`::`WorkflowEnabledUpdate`; _mediaType=nothing) -> `Workflow`, `OpenAPI.Clients.ApiResponse` <br/>
> `set_workflow_enabled_api`(_api::`WorkflowsApi`, response_stream::`Channel`, `workflow_id`::`String`, `workflow_enabled_update`::`WorkflowEnabledUpdate`; _mediaType=nothing) -> `Channel`{ `Workflow` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`WorkflowsApi`** | API context | 
**`workflow_id`** | **`String`** |  |
**`workflow_enabled_update`** | [**`WorkflowEnabledUpdate`**](WorkflowEnabledUpdate.md) |  |

### Return type

[**`Workflow`**](Workflow.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

