# RfqApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**convert_rfq**](RfqApi.md#convert_rfq) | **POST** /api/v1/rfqs/{rfq_id}/convert | Convert an RFQ into a draft purchase order using the quoted unit prices (falling back to the requested prices, then leaving them blank). Marks the RFQ as &#x60;converted&#x60;.
[**create_rfq**](RfqApi.md#create_rfq) | **POST** /api/v1/rfqs | 
[**delete_rfq**](RfqApi.md#delete_rfq) | **DELETE** /api/v1/rfqs/{rfq_id} | 
[**get_rfq**](RfqApi.md#get_rfq) | **GET** /api/v1/rfqs/{rfq_id} | 
[**list_rfqs**](RfqApi.md#list_rfqs) | **GET** /api/v1/rfqs/ | 
[**update_rfq**](RfqApi.md#update_rfq) | **PUT** /api/v1/rfqs/{rfq_id} | 
[**update_rfq_status**](RfqApi.md#update_rfq_status) | **PUT** /api/v1/rfqs/{rfq_id}/status | 


# **convert_rfq**
> `convert_rfq`(_api::`RfqApi`, `rfq_id`::`String`; _mediaType=nothing) -> `Any`, `OpenAPI.Clients.ApiResponse` <br/>
> `convert_rfq`(_api::`RfqApi`, response_stream::`Channel`, `rfq_id`::`String`; _mediaType=nothing) -> `Channel`{ `Any` }, `OpenAPI.Clients.ApiResponse`

Convert an RFQ into a draft purchase order using the quoted unit prices (falling back to the requested prices, then leaving them blank). Marks the RFQ as `converted`.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`RfqApi`** | API context | 
**`rfq_id`** | **`String`** |  |

### Return type

**`Any`**

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **create_rfq**
> `create_rfq`(_api::`RfqApi`, `rfq`::`Rfq`; _mediaType=nothing) -> `Rfq`, `OpenAPI.Clients.ApiResponse` <br/>
> `create_rfq`(_api::`RfqApi`, response_stream::`Channel`, `rfq`::`Rfq`; _mediaType=nothing) -> `Channel`{ `Rfq` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`RfqApi`** | API context | 
**`rfq`** | [**`Rfq`**](Rfq.md) |  |

### Return type

[**`Rfq`**](Rfq.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **delete_rfq**
> `delete_rfq`(_api::`RfqApi`, `rfq_id`::`String`; _mediaType=nothing) -> `Nothing`, `OpenAPI.Clients.ApiResponse` <br/>
> `delete_rfq`(_api::`RfqApi`, response_stream::`Channel`, `rfq_id`::`String`; _mediaType=nothing) -> `Channel`{ `Nothing` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`RfqApi`** | API context | 
**`rfq_id`** | **`String`** |  |

### Return type

`Nothing`

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **get_rfq**
> `get_rfq`(_api::`RfqApi`, `rfq_id`::`String`; _mediaType=nothing) -> `Rfq`, `OpenAPI.Clients.ApiResponse` <br/>
> `get_rfq`(_api::`RfqApi`, response_stream::`Channel`, `rfq_id`::`String`; _mediaType=nothing) -> `Channel`{ `Rfq` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`RfqApi`** | API context | 
**`rfq_id`** | **`String`** |  |

### Return type

[**`Rfq`**](Rfq.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **list_rfqs**
> `list_rfqs`(_api::`RfqApi`; `page`=nothing, `page_size`=nothing, `status`=nothing, `supplier_name`=nothing, _mediaType=nothing) -> `Vector{Rfq}`, `OpenAPI.Clients.ApiResponse` <br/>
> `list_rfqs`(_api::`RfqApi`, response_stream::`Channel`; `page`=nothing, `page_size`=nothing, `status`=nothing, `supplier_name`=nothing, _mediaType=nothing) -> `Channel`{ `Vector{Rfq}` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`RfqApi`** | API context | 

### Optional Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **`page`** | **`Int64`** |  | [default to nothing]
 **`page_size`** | **`Int64`** |  | [default to nothing]
 **`status`** | **`String`** |  | [default to nothing]
 **`supplier_name`** | **`String`** |  | [default to nothing]

### Return type

[**`Vector{Rfq}`**](Rfq.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **update_rfq**
> `update_rfq`(_api::`RfqApi`, `rfq_id`::`String`, `body`::`Any`; _mediaType=nothing) -> `Rfq`, `OpenAPI.Clients.ApiResponse` <br/>
> `update_rfq`(_api::`RfqApi`, response_stream::`Channel`, `rfq_id`::`String`, `body`::`Any`; _mediaType=nothing) -> `Channel`{ `Rfq` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`RfqApi`** | API context | 
**`rfq_id`** | **`String`** |  |
**`body`** | **`Any`** |  |

### Return type

[**`Rfq`**](Rfq.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **update_rfq_status**
> `update_rfq_status`(_api::`RfqApi`, `rfq_id`::`String`, `rfq_status_update`::`RfqStatusUpdate`; _mediaType=nothing) -> `Rfq`, `OpenAPI.Clients.ApiResponse` <br/>
> `update_rfq_status`(_api::`RfqApi`, response_stream::`Channel`, `rfq_id`::`String`, `rfq_status_update`::`RfqStatusUpdate`; _mediaType=nothing) -> `Channel`{ `Rfq` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`RfqApi`** | API context | 
**`rfq_id`** | **`String`** |  |
**`rfq_status_update`** | [**`RfqStatusUpdate`**](RfqStatusUpdate.md) |  |

### Return type

[**`Rfq`**](Rfq.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

