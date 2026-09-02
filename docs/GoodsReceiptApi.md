# GoodsReceiptApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_goods_receipt**](GoodsReceiptApi.md#create_goods_receipt) | **POST** /api/v1/goods-receipts | 
[**delete_goods_receipt**](GoodsReceiptApi.md#delete_goods_receipt) | **DELETE** /api/v1/goods-receipts/{goods_receipt_id} | 
[**get_goods_receipt**](GoodsReceiptApi.md#get_goods_receipt) | **GET** /api/v1/goods-receipts/{goods_receipt_id} | 
[**list_goods_receipts**](GoodsReceiptApi.md#list_goods_receipts) | **GET** /api/v1/goods-receipts/ | 


# **create_goods_receipt**
> `create_goods_receipt`(_api::`GoodsReceiptApi`, `goods_receipt`::`GoodsReceipt`; _mediaType=nothing) -> `GoodsReceipt`, `OpenAPI.Clients.ApiResponse` <br/>
> `create_goods_receipt`(_api::`GoodsReceiptApi`, response_stream::`Channel`, `goods_receipt`::`GoodsReceipt`; _mediaType=nothing) -> `Channel`{ `GoodsReceipt` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`GoodsReceiptApi`** | API context | 
**`goods_receipt`** | [**`GoodsReceipt`**](GoodsReceipt.md) |  |

### Return type

[**`GoodsReceipt`**](GoodsReceipt.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **delete_goods_receipt**
> `delete_goods_receipt`(_api::`GoodsReceiptApi`, `goods_receipt_id`::`String`; _mediaType=nothing) -> `Nothing`, `OpenAPI.Clients.ApiResponse` <br/>
> `delete_goods_receipt`(_api::`GoodsReceiptApi`, response_stream::`Channel`, `goods_receipt_id`::`String`; _mediaType=nothing) -> `Channel`{ `Nothing` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`GoodsReceiptApi`** | API context | 
**`goods_receipt_id`** | **`String`** |  |

### Return type

`Nothing`

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **get_goods_receipt**
> `get_goods_receipt`(_api::`GoodsReceiptApi`, `goods_receipt_id`::`String`; _mediaType=nothing) -> `GoodsReceipt`, `OpenAPI.Clients.ApiResponse` <br/>
> `get_goods_receipt`(_api::`GoodsReceiptApi`, response_stream::`Channel`, `goods_receipt_id`::`String`; _mediaType=nothing) -> `Channel`{ `GoodsReceipt` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`GoodsReceiptApi`** | API context | 
**`goods_receipt_id`** | **`String`** |  |

### Return type

[**`GoodsReceipt`**](GoodsReceipt.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **list_goods_receipts**
> `list_goods_receipts`(_api::`GoodsReceiptApi`; `page`=nothing, `page_size`=nothing, `purchase_order_id`=nothing, `supplier_name`=nothing, `warehouse_id`=nothing, _mediaType=nothing) -> `Vector{GoodsReceipt}`, `OpenAPI.Clients.ApiResponse` <br/>
> `list_goods_receipts`(_api::`GoodsReceiptApi`, response_stream::`Channel`; `page`=nothing, `page_size`=nothing, `purchase_order_id`=nothing, `supplier_name`=nothing, `warehouse_id`=nothing, _mediaType=nothing) -> `Channel`{ `Vector{GoodsReceipt}` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`GoodsReceiptApi`** | API context | 

### Optional Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **`page`** | **`Int64`** |  | [default to nothing]
 **`page_size`** | **`Int64`** |  | [default to nothing]
 **`purchase_order_id`** | **`String`** |  | [default to nothing]
 **`supplier_name`** | **`String`** |  | [default to nothing]
 **`warehouse_id`** | **`String`** |  | [default to nothing]

### Return type

[**`Vector{GoodsReceipt}`**](GoodsReceipt.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

