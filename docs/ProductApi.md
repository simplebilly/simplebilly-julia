# ProductApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_product_api**](ProductApi.md#create_product_api) | **POST** /api/v1/products | 
[**delete_product_api**](ProductApi.md#delete_product_api) | **DELETE** /api/v1/products/{product_id} | 
[**get_product_api**](ProductApi.md#get_product_api) | **GET** /api/v1/products/{product_id} | 
[**get_product_stock_api**](ProductApi.md#get_product_stock_api) | **GET** /api/v1/products/{product_id}/stock | 
[**get_products_api**](ProductApi.md#get_products_api) | **GET** /api/v1/products/ | 
[**list_low_stock_products_api**](ProductApi.md#list_low_stock_products_api) | **GET** /api/v1/products/low-stock | 
[**product_restore**](ProductApi.md#product_restore) | **POST** /api/v1/products/{product_id}/restore | 
[**update_product_api**](ProductApi.md#update_product_api) | **PUT** /api/v1/products/{product_id} | 
[**update_product_stock_api**](ProductApi.md#update_product_stock_api) | **PUT** /api/v1/products/{product_id}/stock | 


# **create_product_api**
> `create_product_api`(_api::`ProductApi`, `product_create`::`ProductCreate`; _mediaType=nothing) -> `Product`, `OpenAPI.Clients.ApiResponse` <br/>
> `create_product_api`(_api::`ProductApi`, response_stream::`Channel`, `product_create`::`ProductCreate`; _mediaType=nothing) -> `Channel`{ `Product` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ProductApi`** | API context | 
**`product_create`** | [**`ProductCreate`**](ProductCreate.md) |  |

### Return type

[**`Product`**](Product.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **delete_product_api**
> `delete_product_api`(_api::`ProductApi`, `product_id`::`String`; _mediaType=nothing) -> `Nothing`, `OpenAPI.Clients.ApiResponse` <br/>
> `delete_product_api`(_api::`ProductApi`, response_stream::`Channel`, `product_id`::`String`; _mediaType=nothing) -> `Channel`{ `Nothing` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ProductApi`** | API context | 
**`product_id`** | **`String`** |  |

### Return type

`Nothing`

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **get_product_api**
> `get_product_api`(_api::`ProductApi`, `product_id`::`String`; _mediaType=nothing) -> `Product`, `OpenAPI.Clients.ApiResponse` <br/>
> `get_product_api`(_api::`ProductApi`, response_stream::`Channel`, `product_id`::`String`; _mediaType=nothing) -> `Channel`{ `Product` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ProductApi`** | API context | 
**`product_id`** | **`String`** |  |

### Return type

[**`Product`**](Product.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **get_product_stock_api**
> `get_product_stock_api`(_api::`ProductApi`, `product_id`::`String`; _mediaType=nothing) -> `ProductStock`, `OpenAPI.Clients.ApiResponse` <br/>
> `get_product_stock_api`(_api::`ProductApi`, response_stream::`Channel`, `product_id`::`String`; _mediaType=nothing) -> `Channel`{ `ProductStock` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ProductApi`** | API context | 
**`product_id`** | **`String`** |  |

### Return type

[**`ProductStock`**](ProductStock.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **get_products_api**
> `get_products_api`(_api::`ProductApi`; `page`=nothing, `page_size`=nothing, `search`=nothing, `include_deleted`=nothing, _mediaType=nothing) -> `Vector{Product}`, `OpenAPI.Clients.ApiResponse` <br/>
> `get_products_api`(_api::`ProductApi`, response_stream::`Channel`; `page`=nothing, `page_size`=nothing, `search`=nothing, `include_deleted`=nothing, _mediaType=nothing) -> `Channel`{ `Vector{Product}` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ProductApi`** | API context | 

### Optional Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **`page`** | **`Int64`** |  | [default to nothing]
 **`page_size`** | **`Int64`** |  | [default to nothing]
 **`search`** | **`String`** |  | [default to nothing]
 **`include_deleted`** | **`Bool`** | Soft-delete entities: set true to include rows with &#x60;deleted_at&#x60; set. | [default to nothing]

### Return type

[**`Vector{Product}`**](Product.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **list_low_stock_products_api**
> `list_low_stock_products_api`(_api::`ProductApi`; `threshold`=nothing, _mediaType=nothing) -> `Vector{ProductStock}`, `OpenAPI.Clients.ApiResponse` <br/>
> `list_low_stock_products_api`(_api::`ProductApi`, response_stream::`Channel`; `threshold`=nothing, _mediaType=nothing) -> `Channel`{ `Vector{ProductStock}` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ProductApi`** | API context | 

### Optional Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **`threshold`** | **`Int64`** |  | [default to nothing]

### Return type

[**`Vector{ProductStock}`**](ProductStock.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **product_restore**
> `product_restore`(_api::`ProductApi`, `product_id`::`String`; _mediaType=nothing) -> `Product`, `OpenAPI.Clients.ApiResponse` <br/>
> `product_restore`(_api::`ProductApi`, response_stream::`Channel`, `product_id`::`String`; _mediaType=nothing) -> `Channel`{ `Product` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ProductApi`** | API context | 
**`product_id`** | **`String`** |  |

### Return type

[**`Product`**](Product.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **update_product_api**
> `update_product_api`(_api::`ProductApi`, `product_id`::`String`, `product_update`::`ProductUpdate`; _mediaType=nothing) -> `Product`, `OpenAPI.Clients.ApiResponse` <br/>
> `update_product_api`(_api::`ProductApi`, response_stream::`Channel`, `product_id`::`String`, `product_update`::`ProductUpdate`; _mediaType=nothing) -> `Channel`{ `Product` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ProductApi`** | API context | 
**`product_id`** | **`String`** |  |
**`product_update`** | [**`ProductUpdate`**](ProductUpdate.md) |  |

### Return type

[**`Product`**](Product.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **update_product_stock_api**
> `update_product_stock_api`(_api::`ProductApi`, `product_id`::`String`, `stock_update_request`::`StockUpdateRequest`; _mediaType=nothing) -> `ProductStock`, `OpenAPI.Clients.ApiResponse` <br/>
> `update_product_stock_api`(_api::`ProductApi`, response_stream::`Channel`, `product_id`::`String`, `stock_update_request`::`StockUpdateRequest`; _mediaType=nothing) -> `Channel`{ `ProductStock` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ProductApi`** | API context | 
**`product_id`** | **`String`** |  |
**`stock_update_request`** | [**`StockUpdateRequest`**](StockUpdateRequest.md) |  |

### Return type

[**`ProductStock`**](ProductStock.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

