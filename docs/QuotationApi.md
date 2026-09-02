# QuotationApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_quotation**](QuotationApi.md#create_quotation) | **POST** /api/v1/quotations | 
[**delete_quotation**](QuotationApi.md#delete_quotation) | **DELETE** /api/v1/quotations/{quotation_id} | 
[**download_quotation_pdf**](QuotationApi.md#download_quotation_pdf) | **GET** /api/v1/quotations/{quotation_id}/pdf | 
[**get_quotation**](QuotationApi.md#get_quotation) | **GET** /api/v1/quotations/{quotation_id} | 
[**list_quotations**](QuotationApi.md#list_quotations) | **GET** /api/v1/quotations/ | 
[**pursue_quotation**](QuotationApi.md#pursue_quotation) | **POST** /api/v1/quotations/{quotation_id}/pursue | 
[**quotation_restore**](QuotationApi.md#quotation_restore) | **POST** /api/v1/quotations/{quotation_id}/restore | 
[**update_quotation**](QuotationApi.md#update_quotation) | **PUT** /api/v1/quotations/{quotation_id} | 


# **create_quotation**
> `create_quotation`(_api::`QuotationApi`, `quotation_create`::`QuotationCreate`; _mediaType=nothing) -> `Quotation`, `OpenAPI.Clients.ApiResponse` <br/>
> `create_quotation`(_api::`QuotationApi`, response_stream::`Channel`, `quotation_create`::`QuotationCreate`; _mediaType=nothing) -> `Channel`{ `Quotation` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`QuotationApi`** | API context | 
**`quotation_create`** | [**`QuotationCreate`**](QuotationCreate.md) |  |

### Return type

[**`Quotation`**](Quotation.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **delete_quotation**
> `delete_quotation`(_api::`QuotationApi`, `quotation_id`::`String`; _mediaType=nothing) -> `Nothing`, `OpenAPI.Clients.ApiResponse` <br/>
> `delete_quotation`(_api::`QuotationApi`, response_stream::`Channel`, `quotation_id`::`String`; _mediaType=nothing) -> `Channel`{ `Nothing` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`QuotationApi`** | API context | 
**`quotation_id`** | **`String`** |  |

### Return type

`Nothing`

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **download_quotation_pdf**
> `download_quotation_pdf`(_api::`QuotationApi`, `quotation_id`::`String`; _mediaType=nothing) -> `Nothing`, `OpenAPI.Clients.ApiResponse` <br/>
> `download_quotation_pdf`(_api::`QuotationApi`, response_stream::`Channel`, `quotation_id`::`String`; _mediaType=nothing) -> `Channel`{ `Nothing` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`QuotationApi`** | API context | 
**`quotation_id`** | **`String`** |  |

### Return type

`Nothing`

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/pdf, application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **get_quotation**
> `get_quotation`(_api::`QuotationApi`, `quotation_id`::`String`; _mediaType=nothing) -> `Quotation`, `OpenAPI.Clients.ApiResponse` <br/>
> `get_quotation`(_api::`QuotationApi`, response_stream::`Channel`, `quotation_id`::`String`; _mediaType=nothing) -> `Channel`{ `Quotation` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`QuotationApi`** | API context | 
**`quotation_id`** | **`String`** |  |

### Return type

[**`Quotation`**](Quotation.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **list_quotations**
> `list_quotations`(_api::`QuotationApi`; `page`=nothing, `page_size`=nothing, `search`=nothing, `include_deleted`=nothing, _mediaType=nothing) -> `Vector{Quotation}`, `OpenAPI.Clients.ApiResponse` <br/>
> `list_quotations`(_api::`QuotationApi`, response_stream::`Channel`; `page`=nothing, `page_size`=nothing, `search`=nothing, `include_deleted`=nothing, _mediaType=nothing) -> `Channel`{ `Vector{Quotation}` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`QuotationApi`** | API context | 

### Optional Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **`page`** | **`Int64`** |  | [default to nothing]
 **`page_size`** | **`Int64`** |  | [default to nothing]
 **`search`** | **`String`** |  | [default to nothing]
 **`include_deleted`** | **`Bool`** | Soft-delete entities: set true to include rows with &#x60;deleted_at&#x60; set. | [default to nothing]

### Return type

[**`Vector{Quotation}`**](Quotation.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **pursue_quotation**
> `pursue_quotation`(_api::`QuotationApi`, `quotation_id`::`String`; _mediaType=nothing) -> `OrderConfirmation`, `OpenAPI.Clients.ApiResponse` <br/>
> `pursue_quotation`(_api::`QuotationApi`, response_stream::`Channel`, `quotation_id`::`String`; _mediaType=nothing) -> `Channel`{ `OrderConfirmation` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`QuotationApi`** | API context | 
**`quotation_id`** | **`String`** |  |

### Return type

[**`OrderConfirmation`**](OrderConfirmation.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **quotation_restore**
> `quotation_restore`(_api::`QuotationApi`, `quotation_id`::`String`; _mediaType=nothing) -> `Quotation`, `OpenAPI.Clients.ApiResponse` <br/>
> `quotation_restore`(_api::`QuotationApi`, response_stream::`Channel`, `quotation_id`::`String`; _mediaType=nothing) -> `Channel`{ `Quotation` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`QuotationApi`** | API context | 
**`quotation_id`** | **`String`** |  |

### Return type

[**`Quotation`**](Quotation.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **update_quotation**
> `update_quotation`(_api::`QuotationApi`, `quotation_id`::`String`, `body`::`Any`; _mediaType=nothing) -> `Quotation`, `OpenAPI.Clients.ApiResponse` <br/>
> `update_quotation`(_api::`QuotationApi`, response_stream::`Channel`, `quotation_id`::`String`, `body`::`Any`; _mediaType=nothing) -> `Channel`{ `Quotation` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`QuotationApi`** | API context | 
**`quotation_id`** | **`String`** |  |
**`body`** | **`Any`** |  |

### Return type

[**`Quotation`**](Quotation.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

