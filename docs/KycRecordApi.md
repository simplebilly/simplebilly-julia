# KycRecordApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_kyc_record**](KycRecordApi.md#create_kyc_record) | **POST** /api/v1/kyc-records | 
[**delete_kyc_record**](KycRecordApi.md#delete_kyc_record) | **DELETE** /api/v1/kyc-records/{id} | 
[**get_kyc_record**](KycRecordApi.md#get_kyc_record) | **GET** /api/v1/kyc-records/{id} | 
[**get_kyc_records**](KycRecordApi.md#get_kyc_records) | **GET** /api/v1/kyc-records/ | 
[**update_kyc_record**](KycRecordApi.md#update_kyc_record) | **PUT** /api/v1/kyc-records/{id} | 


# **create_kyc_record**
> `create_kyc_record`(_api::`KycRecordApi`, `kyc_record_create`::`KycRecordCreate`; _mediaType=nothing) -> `KycRecord`, `OpenAPI.Clients.ApiResponse` <br/>
> `create_kyc_record`(_api::`KycRecordApi`, response_stream::`Channel`, `kyc_record_create`::`KycRecordCreate`; _mediaType=nothing) -> `Channel`{ `KycRecord` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`KycRecordApi`** | API context | 
**`kyc_record_create`** | [**`KycRecordCreate`**](KycRecordCreate.md) |  |

### Return type

[**`KycRecord`**](KycRecord.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **delete_kyc_record**
> `delete_kyc_record`(_api::`KycRecordApi`, `id`::`String`; _mediaType=nothing) -> `Nothing`, `OpenAPI.Clients.ApiResponse` <br/>
> `delete_kyc_record`(_api::`KycRecordApi`, response_stream::`Channel`, `id`::`String`; _mediaType=nothing) -> `Channel`{ `Nothing` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`KycRecordApi`** | API context | 
**`id`** | **`String`** |  |

### Return type

`Nothing`

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **get_kyc_record**
> `get_kyc_record`(_api::`KycRecordApi`, `id`::`String`; _mediaType=nothing) -> `KycRecord`, `OpenAPI.Clients.ApiResponse` <br/>
> `get_kyc_record`(_api::`KycRecordApi`, response_stream::`Channel`, `id`::`String`; _mediaType=nothing) -> `Channel`{ `KycRecord` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`KycRecordApi`** | API context | 
**`id`** | **`String`** |  |

### Return type

[**`KycRecord`**](KycRecord.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **get_kyc_records**
> `get_kyc_records`(_api::`KycRecordApi`; `page`=nothing, `page_size`=nothing, `search`=nothing, `include_deleted`=nothing, _mediaType=nothing) -> `Vector{KycRecord}`, `OpenAPI.Clients.ApiResponse` <br/>
> `get_kyc_records`(_api::`KycRecordApi`, response_stream::`Channel`; `page`=nothing, `page_size`=nothing, `search`=nothing, `include_deleted`=nothing, _mediaType=nothing) -> `Channel`{ `Vector{KycRecord}` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`KycRecordApi`** | API context | 

### Optional Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **`page`** | **`Int64`** |  | [default to nothing]
 **`page_size`** | **`Int64`** |  | [default to nothing]
 **`search`** | **`String`** |  | [default to nothing]
 **`include_deleted`** | **`Bool`** | Soft-delete entities: set true to include rows with &#x60;deleted_at&#x60; set. | [default to nothing]

### Return type

[**`Vector{KycRecord}`**](KycRecord.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **update_kyc_record**
> `update_kyc_record`(_api::`KycRecordApi`, `id`::`String`, `kyc_record_update`::`KycRecordUpdate`; _mediaType=nothing) -> `KycRecord`, `OpenAPI.Clients.ApiResponse` <br/>
> `update_kyc_record`(_api::`KycRecordApi`, response_stream::`Channel`, `id`::`String`, `kyc_record_update`::`KycRecordUpdate`; _mediaType=nothing) -> `Channel`{ `KycRecord` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`KycRecordApi`** | API context | 
**`id`** | **`String`** |  |
**`kyc_record_update`** | [**`KycRecordUpdate`**](KycRecordUpdate.md) |  |

### Return type

[**`KycRecord`**](KycRecord.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

