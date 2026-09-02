# InvoiceApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_invoice**](InvoiceApi.md#create_invoice) | **POST** /api/v1/invoices | 
[**delete_invoice**](InvoiceApi.md#delete_invoice) | **DELETE** /api/v1/invoices/{id} | 
[**download_invoice_pdf**](InvoiceApi.md#download_invoice_pdf) | **GET** /api/v1/invoices/{id}/pdf | 
[**get_invoice**](InvoiceApi.md#get_invoice) | **GET** /api/v1/invoices/{id} | 
[**get_invoice_pdf_url**](InvoiceApi.md#get_invoice_pdf_url) | **GET** /api/v1/invoices/{id}/pdf-url | 
[**get_invoices**](InvoiceApi.md#get_invoices) | **GET** /api/v1/invoices/ | 
[**invoice_restore**](InvoiceApi.md#invoice_restore) | **POST** /api/v1/invoices/{id}/restore | 
[**update_invoice**](InvoiceApi.md#update_invoice) | **PUT** /api/v1/invoices/{id} | 


# **create_invoice**
> `create_invoice`(_api::`InvoiceApi`, `invoice_create`::`InvoiceCreate`; _mediaType=nothing) -> `Invoice`, `OpenAPI.Clients.ApiResponse` <br/>
> `create_invoice`(_api::`InvoiceApi`, response_stream::`Channel`, `invoice_create`::`InvoiceCreate`; _mediaType=nothing) -> `Channel`{ `Invoice` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`InvoiceApi`** | API context | 
**`invoice_create`** | [**`InvoiceCreate`**](InvoiceCreate.md) |  |

### Return type

[**`Invoice`**](Invoice.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **delete_invoice**
> `delete_invoice`(_api::`InvoiceApi`, `id`::`String`; _mediaType=nothing) -> `Nothing`, `OpenAPI.Clients.ApiResponse` <br/>
> `delete_invoice`(_api::`InvoiceApi`, response_stream::`Channel`, `id`::`String`; _mediaType=nothing) -> `Channel`{ `Nothing` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`InvoiceApi`** | API context | 
**`id`** | **`String`** |  |

### Return type

`Nothing`

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **download_invoice_pdf**
> `download_invoice_pdf`(_api::`InvoiceApi`, `id`::`String`; _mediaType=nothing) -> `Nothing`, `OpenAPI.Clients.ApiResponse` <br/>
> `download_invoice_pdf`(_api::`InvoiceApi`, response_stream::`Channel`, `id`::`String`; _mediaType=nothing) -> `Channel`{ `Nothing` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`InvoiceApi`** | API context | 
**`id`** | **`String`** |  |

### Return type

`Nothing`

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/pdf, application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **get_invoice**
> `get_invoice`(_api::`InvoiceApi`, `id`::`String`; _mediaType=nothing) -> `Invoice`, `OpenAPI.Clients.ApiResponse` <br/>
> `get_invoice`(_api::`InvoiceApi`, response_stream::`Channel`, `id`::`String`; _mediaType=nothing) -> `Channel`{ `Invoice` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`InvoiceApi`** | API context | 
**`id`** | **`String`** |  |

### Return type

[**`Invoice`**](Invoice.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **get_invoice_pdf_url**
> `get_invoice_pdf_url`(_api::`InvoiceApi`, `id`::`String`; _mediaType=nothing) -> `InvoicePdfUrlResponse`, `OpenAPI.Clients.ApiResponse` <br/>
> `get_invoice_pdf_url`(_api::`InvoiceApi`, response_stream::`Channel`, `id`::`String`; _mediaType=nothing) -> `Channel`{ `InvoicePdfUrlResponse` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`InvoiceApi`** | API context | 
**`id`** | **`String`** |  |

### Return type

[**`InvoicePdfUrlResponse`**](InvoicePdfUrlResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **get_invoices**
> `get_invoices`(_api::`InvoiceApi`; `page`=nothing, `page_size`=nothing, `search`=nothing, `include_deleted`=nothing, _mediaType=nothing) -> `Vector{Invoice}`, `OpenAPI.Clients.ApiResponse` <br/>
> `get_invoices`(_api::`InvoiceApi`, response_stream::`Channel`; `page`=nothing, `page_size`=nothing, `search`=nothing, `include_deleted`=nothing, _mediaType=nothing) -> `Channel`{ `Vector{Invoice}` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`InvoiceApi`** | API context | 

### Optional Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **`page`** | **`Int64`** |  | [default to nothing]
 **`page_size`** | **`Int64`** |  | [default to nothing]
 **`search`** | **`String`** |  | [default to nothing]
 **`include_deleted`** | **`Bool`** | Soft-delete entities: set true to include rows with &#x60;deleted_at&#x60; set. | [default to nothing]

### Return type

[**`Vector{Invoice}`**](Invoice.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **invoice_restore**
> `invoice_restore`(_api::`InvoiceApi`, `id`::`String`; _mediaType=nothing) -> `Invoice`, `OpenAPI.Clients.ApiResponse` <br/>
> `invoice_restore`(_api::`InvoiceApi`, response_stream::`Channel`, `id`::`String`; _mediaType=nothing) -> `Channel`{ `Invoice` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`InvoiceApi`** | API context | 
**`id`** | **`String`** |  |

### Return type

[**`Invoice`**](Invoice.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **update_invoice**
> `update_invoice`(_api::`InvoiceApi`, `id`::`String`, `body`::`Any`; _mediaType=nothing) -> `Invoice`, `OpenAPI.Clients.ApiResponse` <br/>
> `update_invoice`(_api::`InvoiceApi`, response_stream::`Channel`, `id`::`String`, `body`::`Any`; _mediaType=nothing) -> `Channel`{ `Invoice` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`InvoiceApi`** | API context | 
**`id`** | **`String`** |  |
**`body`** | **`Any`** |  |

### Return type

[**`Invoice`**](Invoice.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

