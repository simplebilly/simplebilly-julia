# EmissionsApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_emission_entry_api**](EmissionsApi.md#create_emission_entry_api) | **POST** /api/v1/bookkeeping/emissions/entries | 
[**create_emission_target_api**](EmissionsApi.md#create_emission_target_api) | **POST** /api/v1/bookkeeping/emissions/targets | 
[**delete_emission_entry_api**](EmissionsApi.md#delete_emission_entry_api) | **DELETE** /api/v1/bookkeeping/emissions/entries/{id} | 
[**delete_emission_target_api**](EmissionsApi.md#delete_emission_target_api) | **DELETE** /api/v1/bookkeeping/emissions/targets/{id} | 
[**emissions_entries_api**](EmissionsApi.md#emissions_entries_api) | **GET** /api/v1/bookkeeping/emissions/entries | 
[**emissions_export_api**](EmissionsApi.md#emissions_export_api) | **GET** /api/v1/bookkeeping/emissions/export | 
[**emissions_factors_api**](EmissionsApi.md#emissions_factors_api) | **GET** /api/v1/bookkeeping/emissions/factors | 
[**emissions_report_api**](EmissionsApi.md#emissions_report_api) | **GET** /api/v1/bookkeeping/emissions/report | 
[**emissions_targets_api**](EmissionsApi.md#emissions_targets_api) | **GET** /api/v1/bookkeeping/emissions/targets | 


# **create_emission_entry_api**
> `create_emission_entry_api`(_api::`EmissionsApi`, `create_emission_entry`::`CreateEmissionEntry`; _mediaType=nothing) -> `EmissionEntry`, `OpenAPI.Clients.ApiResponse` <br/>
> `create_emission_entry_api`(_api::`EmissionsApi`, response_stream::`Channel`, `create_emission_entry`::`CreateEmissionEntry`; _mediaType=nothing) -> `Channel`{ `EmissionEntry` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`EmissionsApi`** | API context | 
**`create_emission_entry`** | [**`CreateEmissionEntry`**](CreateEmissionEntry.md) |  |

### Return type

[**`EmissionEntry`**](EmissionEntry.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **create_emission_target_api**
> `create_emission_target_api`(_api::`EmissionsApi`, `create_emission_target`::`CreateEmissionTarget`; _mediaType=nothing) -> `EmissionTarget`, `OpenAPI.Clients.ApiResponse` <br/>
> `create_emission_target_api`(_api::`EmissionsApi`, response_stream::`Channel`, `create_emission_target`::`CreateEmissionTarget`; _mediaType=nothing) -> `Channel`{ `EmissionTarget` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`EmissionsApi`** | API context | 
**`create_emission_target`** | [**`CreateEmissionTarget`**](CreateEmissionTarget.md) |  |

### Return type

[**`EmissionTarget`**](EmissionTarget.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **delete_emission_entry_api**
> `delete_emission_entry_api`(_api::`EmissionsApi`, `id`::`String`; _mediaType=nothing) -> `Nothing`, `OpenAPI.Clients.ApiResponse` <br/>
> `delete_emission_entry_api`(_api::`EmissionsApi`, response_stream::`Channel`, `id`::`String`; _mediaType=nothing) -> `Channel`{ `Nothing` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`EmissionsApi`** | API context | 
**`id`** | **`String`** |  |

### Return type

`Nothing`

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **delete_emission_target_api**
> `delete_emission_target_api`(_api::`EmissionsApi`, `id`::`String`; _mediaType=nothing) -> `Nothing`, `OpenAPI.Clients.ApiResponse` <br/>
> `delete_emission_target_api`(_api::`EmissionsApi`, response_stream::`Channel`, `id`::`String`; _mediaType=nothing) -> `Channel`{ `Nothing` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`EmissionsApi`** | API context | 
**`id`** | **`String`** |  |

### Return type

`Nothing`

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **emissions_entries_api**
> `emissions_entries_api`(_api::`EmissionsApi`, `year`::`Int64`; _mediaType=nothing) -> `Vector{EmissionEntry}`, `OpenAPI.Clients.ApiResponse` <br/>
> `emissions_entries_api`(_api::`EmissionsApi`, response_stream::`Channel`, `year`::`Int64`; _mediaType=nothing) -> `Channel`{ `Vector{EmissionEntry}` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`EmissionsApi`** | API context | 
**`year`** | **`Int64`** |  |

### Return type

[**`Vector{EmissionEntry}`**](EmissionEntry.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **emissions_export_api**
> `emissions_export_api`(_api::`EmissionsApi`, `year`::`Int64`; _mediaType=nothing) -> `EmissionsExportResponse`, `OpenAPI.Clients.ApiResponse` <br/>
> `emissions_export_api`(_api::`EmissionsApi`, response_stream::`Channel`, `year`::`Int64`; _mediaType=nothing) -> `Channel`{ `EmissionsExportResponse` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`EmissionsApi`** | API context | 
**`year`** | **`Int64`** |  |

### Return type

[**`EmissionsExportResponse`**](EmissionsExportResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **emissions_factors_api**
> `emissions_factors_api`(_api::`EmissionsApi`; _mediaType=nothing) -> `Vector{EmissionFactorResponse}`, `OpenAPI.Clients.ApiResponse` <br/>
> `emissions_factors_api`(_api::`EmissionsApi`, response_stream::`Channel`; _mediaType=nothing) -> `Channel`{ `Vector{EmissionFactorResponse}` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters
This endpoint does not need any parameter.

### Return type

[**`Vector{EmissionFactorResponse}`**](EmissionFactorResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **emissions_report_api**
> `emissions_report_api`(_api::`EmissionsApi`, `year`::`Int64`; _mediaType=nothing) -> `EmissionsReport`, `OpenAPI.Clients.ApiResponse` <br/>
> `emissions_report_api`(_api::`EmissionsApi`, response_stream::`Channel`, `year`::`Int64`; _mediaType=nothing) -> `Channel`{ `EmissionsReport` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`EmissionsApi`** | API context | 
**`year`** | **`Int64`** |  |

### Return type

[**`EmissionsReport`**](EmissionsReport.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **emissions_targets_api**
> `emissions_targets_api`(_api::`EmissionsApi`; _mediaType=nothing) -> `Vector{EmissionTarget}`, `OpenAPI.Clients.ApiResponse` <br/>
> `emissions_targets_api`(_api::`EmissionsApi`, response_stream::`Channel`; _mediaType=nothing) -> `Channel`{ `Vector{EmissionTarget}` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters
This endpoint does not need any parameter.

### Return type

[**`Vector{EmissionTarget}`**](EmissionTarget.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

