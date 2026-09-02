# ProductAttributeApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_product_attribute**](ProductAttributeApi.md#create_product_attribute) | **POST** /api/v1/product-attributes | 
[**delete_product_attribute**](ProductAttributeApi.md#delete_product_attribute) | **DELETE** /api/v1/product-attributes/{attribute_id} | 
[**get_product_attribute**](ProductAttributeApi.md#get_product_attribute) | **GET** /api/v1/product-attributes/{attribute_id} | 
[**list_product_attributes**](ProductAttributeApi.md#list_product_attributes) | **GET** /api/v1/product-attributes/ | 
[**update_product_attribute**](ProductAttributeApi.md#update_product_attribute) | **PUT** /api/v1/product-attributes/{attribute_id} | 


# **create_product_attribute**
> `create_product_attribute`(_api::`ProductAttributeApi`, `product_attribute_create`::`ProductAttributeCreate`; _mediaType=nothing) -> `ProductAttribute`, `OpenAPI.Clients.ApiResponse` <br/>
> `create_product_attribute`(_api::`ProductAttributeApi`, response_stream::`Channel`, `product_attribute_create`::`ProductAttributeCreate`; _mediaType=nothing) -> `Channel`{ `ProductAttribute` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ProductAttributeApi`** | API context | 
**`product_attribute_create`** | [**`ProductAttributeCreate`**](ProductAttributeCreate.md) |  |

### Return type

[**`ProductAttribute`**](ProductAttribute.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **delete_product_attribute**
> `delete_product_attribute`(_api::`ProductAttributeApi`, `attribute_id`::`String`; _mediaType=nothing) -> `Nothing`, `OpenAPI.Clients.ApiResponse` <br/>
> `delete_product_attribute`(_api::`ProductAttributeApi`, response_stream::`Channel`, `attribute_id`::`String`; _mediaType=nothing) -> `Channel`{ `Nothing` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ProductAttributeApi`** | API context | 
**`attribute_id`** | **`String`** |  |

### Return type

`Nothing`

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **get_product_attribute**
> `get_product_attribute`(_api::`ProductAttributeApi`, `attribute_id`::`String`; _mediaType=nothing) -> `ProductAttribute`, `OpenAPI.Clients.ApiResponse` <br/>
> `get_product_attribute`(_api::`ProductAttributeApi`, response_stream::`Channel`, `attribute_id`::`String`; _mediaType=nothing) -> `Channel`{ `ProductAttribute` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ProductAttributeApi`** | API context | 
**`attribute_id`** | **`String`** |  |

### Return type

[**`ProductAttribute`**](ProductAttribute.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **list_product_attributes**
> `list_product_attributes`(_api::`ProductAttributeApi`; `page`=nothing, `page_size`=nothing, `product_id`=nothing, `is_filterable`=nothing, `search`=nothing, _mediaType=nothing) -> `Vector{ProductAttribute}`, `OpenAPI.Clients.ApiResponse` <br/>
> `list_product_attributes`(_api::`ProductAttributeApi`, response_stream::`Channel`; `page`=nothing, `page_size`=nothing, `product_id`=nothing, `is_filterable`=nothing, `search`=nothing, _mediaType=nothing) -> `Channel`{ `Vector{ProductAttribute}` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ProductAttributeApi`** | API context | 

### Optional Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **`page`** | **`Int64`** |  | [default to nothing]
 **`page_size`** | **`Int64`** |  | [default to nothing]
 **`product_id`** | **`String`** |  | [default to nothing]
 **`is_filterable`** | **`Bool`** |  | [default to nothing]
 **`search`** | **`String`** |  | [default to nothing]

### Return type

[**`Vector{ProductAttribute}`**](ProductAttribute.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **update_product_attribute**
> `update_product_attribute`(_api::`ProductAttributeApi`, `attribute_id`::`String`, `product_attribute_update`::`ProductAttributeUpdate`; _mediaType=nothing) -> `ProductAttribute`, `OpenAPI.Clients.ApiResponse` <br/>
> `update_product_attribute`(_api::`ProductAttributeApi`, response_stream::`Channel`, `attribute_id`::`String`, `product_attribute_update`::`ProductAttributeUpdate`; _mediaType=nothing) -> `Channel`{ `ProductAttribute` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ProductAttributeApi`** | API context | 
**`attribute_id`** | **`String`** |  |
**`product_attribute_update`** | [**`ProductAttributeUpdate`**](ProductAttributeUpdate.md) |  |

### Return type

[**`ProductAttribute`**](ProductAttribute.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

