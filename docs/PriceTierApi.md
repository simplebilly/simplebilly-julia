# PriceTierApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_price_tier**](PriceTierApi.md#create_price_tier) | **POST** /api/v1/price-tiers | 
[**delete_price_tier**](PriceTierApi.md#delete_price_tier) | **DELETE** /api/v1/price-tiers/{price_tier_id} | 
[**get_price_tier**](PriceTierApi.md#get_price_tier) | **GET** /api/v1/price-tiers/{price_tier_id} | 
[**get_resolved_price**](PriceTierApi.md#get_resolved_price) | **GET** /api/v1/price-tiers/resolved | 
[**list_price_tiers**](PriceTierApi.md#list_price_tiers) | **GET** /api/v1/price-tiers/ | 
[**update_price_tier**](PriceTierApi.md#update_price_tier) | **PUT** /api/v1/price-tiers/{price_tier_id} | 


# **create_price_tier**
> `create_price_tier`(_api::`PriceTierApi`, `price_tier_create`::`PriceTierCreate`; _mediaType=nothing) -> `PriceTier`, `OpenAPI.Clients.ApiResponse` <br/>
> `create_price_tier`(_api::`PriceTierApi`, response_stream::`Channel`, `price_tier_create`::`PriceTierCreate`; _mediaType=nothing) -> `Channel`{ `PriceTier` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`PriceTierApi`** | API context | 
**`price_tier_create`** | [**`PriceTierCreate`**](PriceTierCreate.md) |  |

### Return type

[**`PriceTier`**](PriceTier.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **delete_price_tier**
> `delete_price_tier`(_api::`PriceTierApi`, `price_tier_id`::`String`; _mediaType=nothing) -> `Nothing`, `OpenAPI.Clients.ApiResponse` <br/>
> `delete_price_tier`(_api::`PriceTierApi`, response_stream::`Channel`, `price_tier_id`::`String`; _mediaType=nothing) -> `Channel`{ `Nothing` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`PriceTierApi`** | API context | 
**`price_tier_id`** | **`String`** |  |

### Return type

`Nothing`

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **get_price_tier**
> `get_price_tier`(_api::`PriceTierApi`, `price_tier_id`::`String`; _mediaType=nothing) -> `PriceTier`, `OpenAPI.Clients.ApiResponse` <br/>
> `get_price_tier`(_api::`PriceTierApi`, response_stream::`Channel`, `price_tier_id`::`String`; _mediaType=nothing) -> `Channel`{ `PriceTier` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`PriceTierApi`** | API context | 
**`price_tier_id`** | **`String`** |  |

### Return type

[**`PriceTier`**](PriceTier.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **get_resolved_price**
> `get_resolved_price`(_api::`PriceTierApi`, `product_id`::`String`; `quantity`=nothing, `contact_id`=nothing, _mediaType=nothing) -> `ResolvedPriceResponse`, `OpenAPI.Clients.ApiResponse` <br/>
> `get_resolved_price`(_api::`PriceTierApi`, response_stream::`Channel`, `product_id`::`String`; `quantity`=nothing, `contact_id`=nothing, _mediaType=nothing) -> `Channel`{ `ResolvedPriceResponse` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`PriceTierApi`** | API context | 
**`product_id`** | **`String`** |  |

### Optional Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **`quantity`** | **`Int64`** |  | [default to nothing]
 **`contact_id`** | **`String`** | Contact used to match customer-group-scoped tiers. | [default to nothing]

### Return type

[**`ResolvedPriceResponse`**](ResolvedPriceResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **list_price_tiers**
> `list_price_tiers`(_api::`PriceTierApi`; `page`=nothing, `page_size`=nothing, `product_id`=nothing, `customer_group_id`=nothing, _mediaType=nothing) -> `Vector{PriceTier}`, `OpenAPI.Clients.ApiResponse` <br/>
> `list_price_tiers`(_api::`PriceTierApi`, response_stream::`Channel`; `page`=nothing, `page_size`=nothing, `product_id`=nothing, `customer_group_id`=nothing, _mediaType=nothing) -> `Channel`{ `Vector{PriceTier}` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`PriceTierApi`** | API context | 

### Optional Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **`page`** | **`Int64`** |  | [default to nothing]
 **`page_size`** | **`Int64`** |  | [default to nothing]
 **`product_id`** | **`String`** |  | [default to nothing]
 **`customer_group_id`** | **`String`** |  | [default to nothing]

### Return type

[**`Vector{PriceTier}`**](PriceTier.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **update_price_tier**
> `update_price_tier`(_api::`PriceTierApi`, `price_tier_id`::`String`, `price_tier_update`::`PriceTierUpdate`; _mediaType=nothing) -> `PriceTier`, `OpenAPI.Clients.ApiResponse` <br/>
> `update_price_tier`(_api::`PriceTierApi`, response_stream::`Channel`, `price_tier_id`::`String`, `price_tier_update`::`PriceTierUpdate`; _mediaType=nothing) -> `Channel`{ `PriceTier` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`PriceTierApi`** | API context | 
**`price_tier_id`** | **`String`** |  |
**`price_tier_update`** | [**`PriceTierUpdate`**](PriceTierUpdate.md) |  |

### Return type

[**`PriceTier`**](PriceTier.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

