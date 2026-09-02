# ProductVariantApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_product_variant**](ProductVariantApi.md#create_product_variant) | **POST** /api/v1/product-variants | 
[**delete_product_variant**](ProductVariantApi.md#delete_product_variant) | **DELETE** /api/v1/product-variants/{variant_id} | 
[**generate_product_variants**](ProductVariantApi.md#generate_product_variants) | **POST** /api/v1/product-variants/generate | 
[**get_product_variant**](ProductVariantApi.md#get_product_variant) | **GET** /api/v1/product-variants/{variant_id} | 
[**list_product_variants**](ProductVariantApi.md#list_product_variants) | **GET** /api/v1/product-variants/ | 
[**update_product_variant**](ProductVariantApi.md#update_product_variant) | **PUT** /api/v1/product-variants/{variant_id} | 


# **create_product_variant**
> `create_product_variant`(_api::`ProductVariantApi`, `product_variant`::`ProductVariant`; _mediaType=nothing) -> `ProductVariant`, `OpenAPI.Clients.ApiResponse` <br/>
> `create_product_variant`(_api::`ProductVariantApi`, response_stream::`Channel`, `product_variant`::`ProductVariant`; _mediaType=nothing) -> `Channel`{ `ProductVariant` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ProductVariantApi`** | API context | 
**`product_variant`** | [**`ProductVariant`**](ProductVariant.md) |  |

### Return type

[**`ProductVariant`**](ProductVariant.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **delete_product_variant**
> `delete_product_variant`(_api::`ProductVariantApi`, `variant_id`::`String`; _mediaType=nothing) -> `Nothing`, `OpenAPI.Clients.ApiResponse` <br/>
> `delete_product_variant`(_api::`ProductVariantApi`, response_stream::`Channel`, `variant_id`::`String`; _mediaType=nothing) -> `Channel`{ `Nothing` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ProductVariantApi`** | API context | 
**`variant_id`** | **`String`** |  |

### Return type

`Nothing`

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **generate_product_variants**
> `generate_product_variants`(_api::`ProductVariantApi`, `generate_variants_request`::`GenerateVariantsRequest`; _mediaType=nothing) -> `Vector{ProductVariant}`, `OpenAPI.Clients.ApiResponse` <br/>
> `generate_product_variants`(_api::`ProductVariantApi`, response_stream::`Channel`, `generate_variants_request`::`GenerateVariantsRequest`; _mediaType=nothing) -> `Channel`{ `Vector{ProductVariant}` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ProductVariantApi`** | API context | 
**`generate_variants_request`** | [**`GenerateVariantsRequest`**](GenerateVariantsRequest.md) |  |

### Return type

[**`Vector{ProductVariant}`**](ProductVariant.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **get_product_variant**
> `get_product_variant`(_api::`ProductVariantApi`, `variant_id`::`String`; _mediaType=nothing) -> `ProductVariant`, `OpenAPI.Clients.ApiResponse` <br/>
> `get_product_variant`(_api::`ProductVariantApi`, response_stream::`Channel`, `variant_id`::`String`; _mediaType=nothing) -> `Channel`{ `ProductVariant` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ProductVariantApi`** | API context | 
**`variant_id`** | **`String`** |  |

### Return type

[**`ProductVariant`**](ProductVariant.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **list_product_variants**
> `list_product_variants`(_api::`ProductVariantApi`; `page`=nothing, `page_size`=nothing, `product_id`=nothing, `is_active`=nothing, _mediaType=nothing) -> `Vector{ProductVariant}`, `OpenAPI.Clients.ApiResponse` <br/>
> `list_product_variants`(_api::`ProductVariantApi`, response_stream::`Channel`; `page`=nothing, `page_size`=nothing, `product_id`=nothing, `is_active`=nothing, _mediaType=nothing) -> `Channel`{ `Vector{ProductVariant}` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ProductVariantApi`** | API context | 

### Optional Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **`page`** | **`Int64`** |  | [default to nothing]
 **`page_size`** | **`Int64`** |  | [default to nothing]
 **`product_id`** | **`String`** |  | [default to nothing]
 **`is_active`** | **`Bool`** |  | [default to nothing]

### Return type

[**`Vector{ProductVariant}`**](ProductVariant.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **update_product_variant**
> `update_product_variant`(_api::`ProductVariantApi`, `variant_id`::`String`, `body`::`Any`; _mediaType=nothing) -> `ProductVariant`, `OpenAPI.Clients.ApiResponse` <br/>
> `update_product_variant`(_api::`ProductVariantApi`, response_stream::`Channel`, `variant_id`::`String`, `body`::`Any`; _mediaType=nothing) -> `Channel`{ `ProductVariant` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ProductVariantApi`** | API context | 
**`variant_id`** | **`String`** |  |
**`body`** | **`Any`** |  |

### Return type

[**`ProductVariant`**](ProductVariant.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

