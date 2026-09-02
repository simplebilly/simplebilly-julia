# InstituteProfileApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_institute_profile**](InstituteProfileApi.md#get_institute_profile) | **GET** /api/v1/institute-profile | Current institute profile (created with defaults when missing).
[**update_institute_profile**](InstituteProfileApi.md#update_institute_profile) | **PUT** /api/v1/institute-profile | Update the institute profile (institute_type and/or kapitalmarktorientiert).


# **get_institute_profile**
> `get_institute_profile`(_api::`InstituteProfileApi`; _mediaType=nothing) -> `InstituteProfile`, `OpenAPI.Clients.ApiResponse` <br/>
> `get_institute_profile`(_api::`InstituteProfileApi`, response_stream::`Channel`; _mediaType=nothing) -> `Channel`{ `InstituteProfile` }, `OpenAPI.Clients.ApiResponse`

Current institute profile (created with defaults when missing).

### Required Parameters
This endpoint does not need any parameter.

### Return type

[**`InstituteProfile`**](InstituteProfile.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **update_institute_profile**
> `update_institute_profile`(_api::`InstituteProfileApi`, `institute_profile_update`::`InstituteProfileUpdate`; _mediaType=nothing) -> `InstituteProfile`, `OpenAPI.Clients.ApiResponse` <br/>
> `update_institute_profile`(_api::`InstituteProfileApi`, response_stream::`Channel`, `institute_profile_update`::`InstituteProfileUpdate`; _mediaType=nothing) -> `Channel`{ `InstituteProfile` }, `OpenAPI.Clients.ApiResponse`

Update the institute profile (institute_type and/or kapitalmarktorientiert).

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`InstituteProfileApi`** | API context | 
**`institute_profile_update`** | [**`InstituteProfileUpdate`**](InstituteProfileUpdate.md) |  |

### Return type

[**`InstituteProfile`**](InstituteProfile.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

