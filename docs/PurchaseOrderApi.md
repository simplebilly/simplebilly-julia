# PurchaseOrderApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_purchase_order**](PurchaseOrderApi.md#create_purchase_order) | **POST** /api/v1/purchase-orders | 
[**delete_purchase_order**](PurchaseOrderApi.md#delete_purchase_order) | **DELETE** /api/v1/purchase-orders/{purchase_order_id} | 
[**get_purchase_order**](PurchaseOrderApi.md#get_purchase_order) | **GET** /api/v1/purchase-orders/{purchase_order_id} | 
[**list_purchase_orders**](PurchaseOrderApi.md#list_purchase_orders) | **GET** /api/v1/purchase-orders/ | 
[**match_invoice**](PurchaseOrderApi.md#match_invoice) | **POST** /api/v1/purchase-orders/{purchase_order_id}/match-invoice | 3-way invoice check (Rechnungsprüfung): compares the purchase order line items, the quantities received via goods receipts, and the supplier invoice line items, reporting quantity and price variances per product.
[**update_purchase_order**](PurchaseOrderApi.md#update_purchase_order) | **PUT** /api/v1/purchase-orders/{purchase_order_id} | 
[**update_purchase_order_status**](PurchaseOrderApi.md#update_purchase_order_status) | **PUT** /api/v1/purchase-orders/{purchase_order_id}/status | 


# **create_purchase_order**
> `create_purchase_order`(_api::`PurchaseOrderApi`, `purchase_order`::`PurchaseOrder`; _mediaType=nothing) -> `PurchaseOrder`, `OpenAPI.Clients.ApiResponse` <br/>
> `create_purchase_order`(_api::`PurchaseOrderApi`, response_stream::`Channel`, `purchase_order`::`PurchaseOrder`; _mediaType=nothing) -> `Channel`{ `PurchaseOrder` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`PurchaseOrderApi`** | API context | 
**`purchase_order`** | [**`PurchaseOrder`**](PurchaseOrder.md) |  |

### Return type

[**`PurchaseOrder`**](PurchaseOrder.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **delete_purchase_order**
> `delete_purchase_order`(_api::`PurchaseOrderApi`, `purchase_order_id`::`String`; _mediaType=nothing) -> `Nothing`, `OpenAPI.Clients.ApiResponse` <br/>
> `delete_purchase_order`(_api::`PurchaseOrderApi`, response_stream::`Channel`, `purchase_order_id`::`String`; _mediaType=nothing) -> `Channel`{ `Nothing` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`PurchaseOrderApi`** | API context | 
**`purchase_order_id`** | **`String`** |  |

### Return type

`Nothing`

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **get_purchase_order**
> `get_purchase_order`(_api::`PurchaseOrderApi`, `purchase_order_id`::`String`; _mediaType=nothing) -> `PurchaseOrder`, `OpenAPI.Clients.ApiResponse` <br/>
> `get_purchase_order`(_api::`PurchaseOrderApi`, response_stream::`Channel`, `purchase_order_id`::`String`; _mediaType=nothing) -> `Channel`{ `PurchaseOrder` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`PurchaseOrderApi`** | API context | 
**`purchase_order_id`** | **`String`** |  |

### Return type

[**`PurchaseOrder`**](PurchaseOrder.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **list_purchase_orders**
> `list_purchase_orders`(_api::`PurchaseOrderApi`; `page`=nothing, `page_size`=nothing, `status`=nothing, `supplier_name`=nothing, `search`=nothing, _mediaType=nothing) -> `Vector{PurchaseOrder}`, `OpenAPI.Clients.ApiResponse` <br/>
> `list_purchase_orders`(_api::`PurchaseOrderApi`, response_stream::`Channel`; `page`=nothing, `page_size`=nothing, `status`=nothing, `supplier_name`=nothing, `search`=nothing, _mediaType=nothing) -> `Channel`{ `Vector{PurchaseOrder}` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`PurchaseOrderApi`** | API context | 

### Optional Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **`page`** | **`Int64`** |  | [default to nothing]
 **`page_size`** | **`Int64`** |  | [default to nothing]
 **`status`** | **`String`** |  | [default to nothing]
 **`supplier_name`** | **`String`** |  | [default to nothing]
 **`search`** | **`String`** |  | [default to nothing]

### Return type

[**`Vector{PurchaseOrder}`**](PurchaseOrder.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **match_invoice**
> `match_invoice`(_api::`PurchaseOrderApi`, `purchase_order_id`::`String`, `invoice_match_request`::`InvoiceMatchRequest`; _mediaType=nothing) -> `Any`, `OpenAPI.Clients.ApiResponse` <br/>
> `match_invoice`(_api::`PurchaseOrderApi`, response_stream::`Channel`, `purchase_order_id`::`String`, `invoice_match_request`::`InvoiceMatchRequest`; _mediaType=nothing) -> `Channel`{ `Any` }, `OpenAPI.Clients.ApiResponse`

3-way invoice check (Rechnungsprüfung): compares the purchase order line items, the quantities received via goods receipts, and the supplier invoice line items, reporting quantity and price variances per product.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`PurchaseOrderApi`** | API context | 
**`purchase_order_id`** | **`String`** |  |
**`invoice_match_request`** | [**`InvoiceMatchRequest`**](InvoiceMatchRequest.md) |  |

### Return type

**`Any`**

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **update_purchase_order**
> `update_purchase_order`(_api::`PurchaseOrderApi`, `purchase_order_id`::`String`, `body`::`Any`; _mediaType=nothing) -> `PurchaseOrder`, `OpenAPI.Clients.ApiResponse` <br/>
> `update_purchase_order`(_api::`PurchaseOrderApi`, response_stream::`Channel`, `purchase_order_id`::`String`, `body`::`Any`; _mediaType=nothing) -> `Channel`{ `PurchaseOrder` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`PurchaseOrderApi`** | API context | 
**`purchase_order_id`** | **`String`** |  |
**`body`** | **`Any`** |  |

### Return type

[**`PurchaseOrder`**](PurchaseOrder.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **update_purchase_order_status**
> `update_purchase_order_status`(_api::`PurchaseOrderApi`, `purchase_order_id`::`String`, `purchase_order_status_update`::`PurchaseOrderStatusUpdate`; _mediaType=nothing) -> `PurchaseOrder`, `OpenAPI.Clients.ApiResponse` <br/>
> `update_purchase_order_status`(_api::`PurchaseOrderApi`, response_stream::`Channel`, `purchase_order_id`::`String`, `purchase_order_status_update`::`PurchaseOrderStatusUpdate`; _mediaType=nothing) -> `Channel`{ `PurchaseOrder` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`PurchaseOrderApi`** | API context | 
**`purchase_order_id`** | **`String`** |  |
**`purchase_order_status_update`** | [**`PurchaseOrderStatusUpdate`**](PurchaseOrderStatusUpdate.md) |  |

### Return type

[**`PurchaseOrder`**](PurchaseOrder.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

