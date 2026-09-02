# ProposeAssignmentsApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**propose_assignments_api**](ProposeAssignmentsApi.md#propose_assignments_api) | **GET** /api/v1/bookkeeping/propose-assignments | 


# **propose_assignments_api**
> `propose_assignments_api`(_api::`ProposeAssignmentsApi`; `min_confidence`=nothing, `customer_id`=nothing, _mediaType=nothing) -> `Vector{ProposedAssignment}`, `OpenAPI.Clients.ApiResponse` <br/>
> `propose_assignments_api`(_api::`ProposeAssignmentsApi`, response_stream::`Channel`; `min_confidence`=nothing, `customer_id`=nothing, _mediaType=nothing) -> `Channel`{ `Vector{ProposedAssignment}` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ProposeAssignmentsApi`** | API context | 

### Optional Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **`min_confidence`** | **`Float64`** |  | [default to nothing]
 **`customer_id`** | **`String`** |  | [default to nothing]

### Return type

[**`Vector{ProposedAssignment}`**](ProposedAssignment.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

