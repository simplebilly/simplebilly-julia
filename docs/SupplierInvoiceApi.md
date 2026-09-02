# SupplierInvoiceApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_supplier_invoice**](SupplierInvoiceApi.md#create_supplier_invoice) | **POST** /api/v1/supplier-invoices | 
[**delete_supplier_invoice**](SupplierInvoiceApi.md#delete_supplier_invoice) | **DELETE** /api/v1/supplier-invoices/{supplier_invoice_id} | 
[**get_supplier_invoice**](SupplierInvoiceApi.md#get_supplier_invoice) | **GET** /api/v1/supplier-invoices/{supplier_invoice_id} | 
[**list_supplier_invoices**](SupplierInvoiceApi.md#list_supplier_invoices) | **GET** /api/v1/supplier-invoices/ | 
[**update_supplier_invoice**](SupplierInvoiceApi.md#update_supplier_invoice) | **PUT** /api/v1/supplier-invoices/{supplier_invoice_id} | 
[**update_supplier_invoice_status**](SupplierInvoiceApi.md#update_supplier_invoice_status) | **PUT** /api/v1/supplier-invoices/{supplier_invoice_id}/status | 


# **create_supplier_invoice**
> `create_supplier_invoice`(_api::`SupplierInvoiceApi`, `supplier_invoice`::`SupplierInvoice`; _mediaType=nothing) -> `SupplierInvoice`, `OpenAPI.Clients.ApiResponse` <br/>
> `create_supplier_invoice`(_api::`SupplierInvoiceApi`, response_stream::`Channel`, `supplier_invoice`::`SupplierInvoice`; _mediaType=nothing) -> `Channel`{ `SupplierInvoice` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`SupplierInvoiceApi`** | API context | 
**`supplier_invoice`** | [**`SupplierInvoice`**](SupplierInvoice.md) |  |

### Return type

[**`SupplierInvoice`**](SupplierInvoice.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **delete_supplier_invoice**
> `delete_supplier_invoice`(_api::`SupplierInvoiceApi`, `supplier_invoice_id`::`String`; _mediaType=nothing) -> `Nothing`, `OpenAPI.Clients.ApiResponse` <br/>
> `delete_supplier_invoice`(_api::`SupplierInvoiceApi`, response_stream::`Channel`, `supplier_invoice_id`::`String`; _mediaType=nothing) -> `Channel`{ `Nothing` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`SupplierInvoiceApi`** | API context | 
**`supplier_invoice_id`** | **`String`** |  |

### Return type

`Nothing`

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **get_supplier_invoice**
> `get_supplier_invoice`(_api::`SupplierInvoiceApi`, `supplier_invoice_id`::`String`; _mediaType=nothing) -> `SupplierInvoice`, `OpenAPI.Clients.ApiResponse` <br/>
> `get_supplier_invoice`(_api::`SupplierInvoiceApi`, response_stream::`Channel`, `supplier_invoice_id`::`String`; _mediaType=nothing) -> `Channel`{ `SupplierInvoice` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`SupplierInvoiceApi`** | API context | 
**`supplier_invoice_id`** | **`String`** |  |

### Return type

[**`SupplierInvoice`**](SupplierInvoice.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **list_supplier_invoices**
> `list_supplier_invoices`(_api::`SupplierInvoiceApi`; `page`=nothing, `page_size`=nothing, `status`=nothing, `purchase_order_id`=nothing, `supplier_name`=nothing, _mediaType=nothing) -> `Vector{SupplierInvoice}`, `OpenAPI.Clients.ApiResponse` <br/>
> `list_supplier_invoices`(_api::`SupplierInvoiceApi`, response_stream::`Channel`; `page`=nothing, `page_size`=nothing, `status`=nothing, `purchase_order_id`=nothing, `supplier_name`=nothing, _mediaType=nothing) -> `Channel`{ `Vector{SupplierInvoice}` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`SupplierInvoiceApi`** | API context | 

### Optional Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **`page`** | **`Int64`** |  | [default to nothing]
 **`page_size`** | **`Int64`** |  | [default to nothing]
 **`status`** | **`String`** |  | [default to nothing]
 **`purchase_order_id`** | **`String`** |  | [default to nothing]
 **`supplier_name`** | **`String`** |  | [default to nothing]

### Return type

[**`Vector{SupplierInvoice}`**](SupplierInvoice.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **update_supplier_invoice**
> `update_supplier_invoice`(_api::`SupplierInvoiceApi`, `supplier_invoice_id`::`String`, `body`::`Any`; _mediaType=nothing) -> `SupplierInvoice`, `OpenAPI.Clients.ApiResponse` <br/>
> `update_supplier_invoice`(_api::`SupplierInvoiceApi`, response_stream::`Channel`, `supplier_invoice_id`::`String`, `body`::`Any`; _mediaType=nothing) -> `Channel`{ `SupplierInvoice` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`SupplierInvoiceApi`** | API context | 
**`supplier_invoice_id`** | **`String`** |  |
**`body`** | **`Any`** |  |

### Return type

[**`SupplierInvoice`**](SupplierInvoice.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **update_supplier_invoice_status**
> `update_supplier_invoice_status`(_api::`SupplierInvoiceApi`, `supplier_invoice_id`::`String`, `supplier_invoice_status_update`::`SupplierInvoiceStatusUpdate`; _mediaType=nothing) -> `SupplierInvoice`, `OpenAPI.Clients.ApiResponse` <br/>
> `update_supplier_invoice_status`(_api::`SupplierInvoiceApi`, response_stream::`Channel`, `supplier_invoice_id`::`String`, `supplier_invoice_status_update`::`SupplierInvoiceStatusUpdate`; _mediaType=nothing) -> `Channel`{ `SupplierInvoice` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`SupplierInvoiceApi`** | API context | 
**`supplier_invoice_id`** | **`String`** |  |
**`supplier_invoice_status_update`** | [**`SupplierInvoiceStatusUpdate`**](SupplierInvoiceStatusUpdate.md) |  |

### Return type

[**`SupplierInvoice`**](SupplierInvoice.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

