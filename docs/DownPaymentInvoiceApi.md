# DownPaymentInvoiceApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**download_down_payment_invoice_pdf**](DownPaymentInvoiceApi.md#download_down_payment_invoice_pdf) | **GET** /api/v1/down-payment-invoices/{id}/pdf | 
[**get_down_payment_invoice**](DownPaymentInvoiceApi.md#get_down_payment_invoice) | **GET** /api/v1/down-payment-invoices/{id} | 
[**list_down_payment_invoices**](DownPaymentInvoiceApi.md#list_down_payment_invoices) | **GET** /api/v1/down-payment-invoices/ | 


# **download_down_payment_invoice_pdf**
> `download_down_payment_invoice_pdf`(_api::`DownPaymentInvoiceApi`, `id`::`String`; _mediaType=nothing) -> `Nothing`, `OpenAPI.Clients.ApiResponse` <br/>
> `download_down_payment_invoice_pdf`(_api::`DownPaymentInvoiceApi`, response_stream::`Channel`, `id`::`String`; _mediaType=nothing) -> `Channel`{ `Nothing` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`DownPaymentInvoiceApi`** | API context | 
**`id`** | **`String`** |  |

### Return type

`Nothing`

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **get_down_payment_invoice**
> `get_down_payment_invoice`(_api::`DownPaymentInvoiceApi`, `id`::`String`; _mediaType=nothing) -> `DownPaymentInvoice`, `OpenAPI.Clients.ApiResponse` <br/>
> `get_down_payment_invoice`(_api::`DownPaymentInvoiceApi`, response_stream::`Channel`, `id`::`String`; _mediaType=nothing) -> `Channel`{ `DownPaymentInvoice` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`DownPaymentInvoiceApi`** | API context | 
**`id`** | **`String`** |  |

### Return type

[**`DownPaymentInvoice`**](DownPaymentInvoice.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **list_down_payment_invoices**
> `list_down_payment_invoices`(_api::`DownPaymentInvoiceApi`; `page`=nothing, `page_size`=nothing, `search`=nothing, `include_deleted`=nothing, _mediaType=nothing) -> `Vector{DownPaymentInvoice}`, `OpenAPI.Clients.ApiResponse` <br/>
> `list_down_payment_invoices`(_api::`DownPaymentInvoiceApi`, response_stream::`Channel`; `page`=nothing, `page_size`=nothing, `search`=nothing, `include_deleted`=nothing, _mediaType=nothing) -> `Channel`{ `Vector{DownPaymentInvoice}` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`DownPaymentInvoiceApi`** | API context | 

### Optional Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **`page`** | **`Int64`** |  | [default to nothing]
 **`page_size`** | **`Int64`** |  | [default to nothing]
 **`search`** | **`String`** |  | [default to nothing]
 **`include_deleted`** | **`Bool`** | Soft-delete entities: set true to include rows with &#x60;deleted_at&#x60; set. | [default to nothing]

### Return type

[**`Vector{DownPaymentInvoice}`**](DownPaymentInvoice.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

