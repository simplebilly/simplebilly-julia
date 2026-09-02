# ProductCategoryApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_product_category**](ProductCategoryApi.md#create_product_category) | **POST** /api/v1/product-categories | 
[**delete_product_category**](ProductCategoryApi.md#delete_product_category) | **DELETE** /api/v1/product-categories/{category_id} | 
[**get_product_category**](ProductCategoryApi.md#get_product_category) | **GET** /api/v1/product-categories/{category_id} | 
[**list_product_categories**](ProductCategoryApi.md#list_product_categories) | **GET** /api/v1/product-categories | 
[**update_product_category**](ProductCategoryApi.md#update_product_category) | **PUT** /api/v1/product-categories/{category_id} | 


# **create_product_category**
> `create_product_category`(_api::`ProductCategoryApi`, `product_category`::`ProductCategory`; _mediaType=nothing) -> `ProductCategory`, `OpenAPI.Clients.ApiResponse` <br/>
> `create_product_category`(_api::`ProductCategoryApi`, response_stream::`Channel`, `product_category`::`ProductCategory`; _mediaType=nothing) -> `Channel`{ `ProductCategory` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ProductCategoryApi`** | API context | 
**`product_category`** | [**`ProductCategory`**](ProductCategory.md) |  |

### Return type

[**`ProductCategory`**](ProductCategory.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **delete_product_category**
> `delete_product_category`(_api::`ProductCategoryApi`, `category_id`::`String`; _mediaType=nothing) -> `Nothing`, `OpenAPI.Clients.ApiResponse` <br/>
> `delete_product_category`(_api::`ProductCategoryApi`, response_stream::`Channel`, `category_id`::`String`; _mediaType=nothing) -> `Channel`{ `Nothing` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ProductCategoryApi`** | API context | 
**`category_id`** | **`String`** |  |

### Return type

`Nothing`

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **get_product_category**
> `get_product_category`(_api::`ProductCategoryApi`, `category_id`::`String`; _mediaType=nothing) -> `ProductCategory`, `OpenAPI.Clients.ApiResponse` <br/>
> `get_product_category`(_api::`ProductCategoryApi`, response_stream::`Channel`, `category_id`::`String`; _mediaType=nothing) -> `Channel`{ `ProductCategory` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ProductCategoryApi`** | API context | 
**`category_id`** | **`String`** |  |

### Return type

[**`ProductCategory`**](ProductCategory.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **list_product_categories**
> `list_product_categories`(_api::`ProductCategoryApi`; _mediaType=nothing) -> `Vector{ProductCategory}`, `OpenAPI.Clients.ApiResponse` <br/>
> `list_product_categories`(_api::`ProductCategoryApi`, response_stream::`Channel`; _mediaType=nothing) -> `Channel`{ `Vector{ProductCategory}` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters
This endpoint does not need any parameter.

### Return type

[**`Vector{ProductCategory}`**](ProductCategory.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **update_product_category**
> `update_product_category`(_api::`ProductCategoryApi`, `category_id`::`String`, `body`::`Any`; _mediaType=nothing) -> `ProductCategory`, `OpenAPI.Clients.ApiResponse` <br/>
> `update_product_category`(_api::`ProductCategoryApi`, response_stream::`Channel`, `category_id`::`String`, `body`::`Any`; _mediaType=nothing) -> `Channel`{ `ProductCategory` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ProductCategoryApi`** | API context | 
**`category_id`** | **`String`** |  |
**`body`** | **`Any`** |  |

### Return type

[**`ProductCategory`**](ProductCategory.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

