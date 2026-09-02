# ProformaInvoiceApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**convert_proforma_to_invoice**](ProformaInvoiceApi.md#convert_proforma_to_invoice) | **POST** /api/v1/proforma-invoices/{proforma_id}/convert | 
[**create_proforma_invoice**](ProformaInvoiceApi.md#create_proforma_invoice) | **POST** /api/v1/proforma-invoices | 
[**delete_proforma_invoice**](ProformaInvoiceApi.md#delete_proforma_invoice) | **DELETE** /api/v1/proforma-invoices/{proforma_id} | 
[**get_proforma_invoice**](ProformaInvoiceApi.md#get_proforma_invoice) | **GET** /api/v1/proforma-invoices/{proforma_id} | 
[**list_proforma_invoices**](ProformaInvoiceApi.md#list_proforma_invoices) | **GET** /api/v1/proforma-invoices/ | 
[**update_proforma_invoice**](ProformaInvoiceApi.md#update_proforma_invoice) | **PUT** /api/v1/proforma-invoices/{proforma_id} | 


# **convert_proforma_to_invoice**
> `convert_proforma_to_invoice`(_api::`ProformaInvoiceApi`, `proforma_id`::`String`; _mediaType=nothing) -> `ConvertResponse`, `OpenAPI.Clients.ApiResponse` <br/>
> `convert_proforma_to_invoice`(_api::`ProformaInvoiceApi`, response_stream::`Channel`, `proforma_id`::`String`; _mediaType=nothing) -> `Channel`{ `ConvertResponse` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ProformaInvoiceApi`** | API context | 
**`proforma_id`** | **`String`** |  |

### Return type

[**`ConvertResponse`**](ConvertResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **create_proforma_invoice**
> `create_proforma_invoice`(_api::`ProformaInvoiceApi`, `proforma_invoice`::`ProformaInvoice`; _mediaType=nothing) -> `ProformaInvoice`, `OpenAPI.Clients.ApiResponse` <br/>
> `create_proforma_invoice`(_api::`ProformaInvoiceApi`, response_stream::`Channel`, `proforma_invoice`::`ProformaInvoice`; _mediaType=nothing) -> `Channel`{ `ProformaInvoice` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ProformaInvoiceApi`** | API context | 
**`proforma_invoice`** | [**`ProformaInvoice`**](ProformaInvoice.md) |  |

### Return type

[**`ProformaInvoice`**](ProformaInvoice.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **delete_proforma_invoice**
> `delete_proforma_invoice`(_api::`ProformaInvoiceApi`, `proforma_id`::`String`; _mediaType=nothing) -> `Nothing`, `OpenAPI.Clients.ApiResponse` <br/>
> `delete_proforma_invoice`(_api::`ProformaInvoiceApi`, response_stream::`Channel`, `proforma_id`::`String`; _mediaType=nothing) -> `Channel`{ `Nothing` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ProformaInvoiceApi`** | API context | 
**`proforma_id`** | **`String`** |  |

### Return type

`Nothing`

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **get_proforma_invoice**
> `get_proforma_invoice`(_api::`ProformaInvoiceApi`, `proforma_id`::`String`; _mediaType=nothing) -> `ProformaInvoice`, `OpenAPI.Clients.ApiResponse` <br/>
> `get_proforma_invoice`(_api::`ProformaInvoiceApi`, response_stream::`Channel`, `proforma_id`::`String`; _mediaType=nothing) -> `Channel`{ `ProformaInvoice` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ProformaInvoiceApi`** | API context | 
**`proforma_id`** | **`String`** |  |

### Return type

[**`ProformaInvoice`**](ProformaInvoice.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **list_proforma_invoices**
> `list_proforma_invoices`(_api::`ProformaInvoiceApi`; `page`=nothing, `page_size`=nothing, `status`=nothing, `customer_id`=nothing, `order_number`=nothing, _mediaType=nothing) -> `Vector{ProformaInvoice}`, `OpenAPI.Clients.ApiResponse` <br/>
> `list_proforma_invoices`(_api::`ProformaInvoiceApi`, response_stream::`Channel`; `page`=nothing, `page_size`=nothing, `status`=nothing, `customer_id`=nothing, `order_number`=nothing, _mediaType=nothing) -> `Channel`{ `Vector{ProformaInvoice}` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ProformaInvoiceApi`** | API context | 

### Optional Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **`page`** | **`Int64`** |  | [default to nothing]
 **`page_size`** | **`Int64`** |  | [default to nothing]
 **`status`** | **`String`** |  | [default to nothing]
 **`customer_id`** | **`String`** |  | [default to nothing]
 **`order_number`** | **`String`** |  | [default to nothing]

### Return type

[**`Vector{ProformaInvoice}`**](ProformaInvoice.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **update_proforma_invoice**
> `update_proforma_invoice`(_api::`ProformaInvoiceApi`, `proforma_id`::`String`, `body`::`Any`; _mediaType=nothing) -> `ProformaInvoice`, `OpenAPI.Clients.ApiResponse` <br/>
> `update_proforma_invoice`(_api::`ProformaInvoiceApi`, response_stream::`Channel`, `proforma_id`::`String`, `body`::`Any`; _mediaType=nothing) -> `Channel`{ `ProformaInvoice` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ProformaInvoiceApi`** | API context | 
**`proforma_id`** | **`String`** |  |
**`body`** | **`Any`** |  |

### Return type

[**`ProformaInvoice`**](ProformaInvoice.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

