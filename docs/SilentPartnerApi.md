# SilentPartnerApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_silent_partner**](SilentPartnerApi.md#create_silent_partner) | **POST** /api/v1/silent-partners | 
[**delete_silent_partner**](SilentPartnerApi.md#delete_silent_partner) | **DELETE** /api/v1/silent-partners/{id} | 
[**get_silent_partner**](SilentPartnerApi.md#get_silent_partner) | **GET** /api/v1/silent-partners/{id} | 
[**get_silent_partners**](SilentPartnerApi.md#get_silent_partners) | **GET** /api/v1/silent-partners/ | 
[**update_silent_partner**](SilentPartnerApi.md#update_silent_partner) | **PUT** /api/v1/silent-partners/{id} | 


# **create_silent_partner**
> `create_silent_partner`(_api::`SilentPartnerApi`, `silent_partner_create`::`SilentPartnerCreate`; _mediaType=nothing) -> `SilentPartner`, `OpenAPI.Clients.ApiResponse` <br/>
> `create_silent_partner`(_api::`SilentPartnerApi`, response_stream::`Channel`, `silent_partner_create`::`SilentPartnerCreate`; _mediaType=nothing) -> `Channel`{ `SilentPartner` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`SilentPartnerApi`** | API context | 
**`silent_partner_create`** | [**`SilentPartnerCreate`**](SilentPartnerCreate.md) |  |

### Return type

[**`SilentPartner`**](SilentPartner.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **delete_silent_partner**
> `delete_silent_partner`(_api::`SilentPartnerApi`, `id`::`String`; _mediaType=nothing) -> `Nothing`, `OpenAPI.Clients.ApiResponse` <br/>
> `delete_silent_partner`(_api::`SilentPartnerApi`, response_stream::`Channel`, `id`::`String`; _mediaType=nothing) -> `Channel`{ `Nothing` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`SilentPartnerApi`** | API context | 
**`id`** | **`String`** |  |

### Return type

`Nothing`

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **get_silent_partner**
> `get_silent_partner`(_api::`SilentPartnerApi`, `id`::`String`; _mediaType=nothing) -> `SilentPartner`, `OpenAPI.Clients.ApiResponse` <br/>
> `get_silent_partner`(_api::`SilentPartnerApi`, response_stream::`Channel`, `id`::`String`; _mediaType=nothing) -> `Channel`{ `SilentPartner` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`SilentPartnerApi`** | API context | 
**`id`** | **`String`** |  |

### Return type

[**`SilentPartner`**](SilentPartner.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **get_silent_partners**
> `get_silent_partners`(_api::`SilentPartnerApi`; `page`=nothing, `page_size`=nothing, `search`=nothing, `include_deleted`=nothing, _mediaType=nothing) -> `Vector{SilentPartner}`, `OpenAPI.Clients.ApiResponse` <br/>
> `get_silent_partners`(_api::`SilentPartnerApi`, response_stream::`Channel`; `page`=nothing, `page_size`=nothing, `search`=nothing, `include_deleted`=nothing, _mediaType=nothing) -> `Channel`{ `Vector{SilentPartner}` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`SilentPartnerApi`** | API context | 

### Optional Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **`page`** | **`Int64`** |  | [default to nothing]
 **`page_size`** | **`Int64`** |  | [default to nothing]
 **`search`** | **`String`** |  | [default to nothing]
 **`include_deleted`** | **`Bool`** | Soft-delete entities: set true to include rows with &#x60;deleted_at&#x60; set. | [default to nothing]

### Return type

[**`Vector{SilentPartner}`**](SilentPartner.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **update_silent_partner**
> `update_silent_partner`(_api::`SilentPartnerApi`, `id`::`String`, `silent_partner_update`::`SilentPartnerUpdate`; _mediaType=nothing) -> `SilentPartner`, `OpenAPI.Clients.ApiResponse` <br/>
> `update_silent_partner`(_api::`SilentPartnerApi`, response_stream::`Channel`, `id`::`String`, `silent_partner_update`::`SilentPartnerUpdate`; _mediaType=nothing) -> `Channel`{ `SilentPartner` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`SilentPartnerApi`** | API context | 
**`id`** | **`String`** |  |
**`silent_partner_update`** | [**`SilentPartnerUpdate`**](SilentPartnerUpdate.md) |  |

### Return type

[**`SilentPartner`**](SilentPartner.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

