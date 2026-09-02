# ShippingRuleApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_shipping_rule**](ShippingRuleApi.md#create_shipping_rule) | **POST** /api/v1/shipping-rules | 
[**delete_shipping_rule**](ShippingRuleApi.md#delete_shipping_rule) | **DELETE** /api/v1/shipping-rules/{rule_id} | 
[**get_shipping_rule**](ShippingRuleApi.md#get_shipping_rule) | **GET** /api/v1/shipping-rules/{rule_id} | 
[**list_shipping_rules**](ShippingRuleApi.md#list_shipping_rules) | **GET** /api/v1/shipping-rules/ | 
[**update_shipping_rule**](ShippingRuleApi.md#update_shipping_rule) | **PUT** /api/v1/shipping-rules/{rule_id} | 


# **create_shipping_rule**
> `create_shipping_rule`(_api::`ShippingRuleApi`, `shipping_rule_create`::`ShippingRuleCreate`; _mediaType=nothing) -> `ShippingRule`, `OpenAPI.Clients.ApiResponse` <br/>
> `create_shipping_rule`(_api::`ShippingRuleApi`, response_stream::`Channel`, `shipping_rule_create`::`ShippingRuleCreate`; _mediaType=nothing) -> `Channel`{ `ShippingRule` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ShippingRuleApi`** | API context | 
**`shipping_rule_create`** | [**`ShippingRuleCreate`**](ShippingRuleCreate.md) |  |

### Return type

[**`ShippingRule`**](ShippingRule.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **delete_shipping_rule**
> `delete_shipping_rule`(_api::`ShippingRuleApi`, `rule_id`::`String`; _mediaType=nothing) -> `Nothing`, `OpenAPI.Clients.ApiResponse` <br/>
> `delete_shipping_rule`(_api::`ShippingRuleApi`, response_stream::`Channel`, `rule_id`::`String`; _mediaType=nothing) -> `Channel`{ `Nothing` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ShippingRuleApi`** | API context | 
**`rule_id`** | **`String`** |  |

### Return type

`Nothing`

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **get_shipping_rule**
> `get_shipping_rule`(_api::`ShippingRuleApi`, `rule_id`::`String`; _mediaType=nothing) -> `ShippingRule`, `OpenAPI.Clients.ApiResponse` <br/>
> `get_shipping_rule`(_api::`ShippingRuleApi`, response_stream::`Channel`, `rule_id`::`String`; _mediaType=nothing) -> `Channel`{ `ShippingRule` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ShippingRuleApi`** | API context | 
**`rule_id`** | **`String`** |  |

### Return type

[**`ShippingRule`**](ShippingRule.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **list_shipping_rules**
> `list_shipping_rules`(_api::`ShippingRuleApi`; `page`=nothing, `page_size`=nothing, `country`=nothing, _mediaType=nothing) -> `Vector{ShippingRule}`, `OpenAPI.Clients.ApiResponse` <br/>
> `list_shipping_rules`(_api::`ShippingRuleApi`, response_stream::`Channel`; `page`=nothing, `page_size`=nothing, `country`=nothing, _mediaType=nothing) -> `Channel`{ `Vector{ShippingRule}` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ShippingRuleApi`** | API context | 

### Optional Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **`page`** | **`Int64`** |  | [default to nothing]
 **`page_size`** | **`Int64`** |  | [default to nothing]
 **`country`** | **`String`** |  | [default to nothing]

### Return type

[**`Vector{ShippingRule}`**](ShippingRule.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **update_shipping_rule**
> `update_shipping_rule`(_api::`ShippingRuleApi`, `rule_id`::`String`, `shipping_rule_update`::`ShippingRuleUpdate`; _mediaType=nothing) -> `ShippingRule`, `OpenAPI.Clients.ApiResponse` <br/>
> `update_shipping_rule`(_api::`ShippingRuleApi`, response_stream::`Channel`, `rule_id`::`String`, `shipping_rule_update`::`ShippingRuleUpdate`; _mediaType=nothing) -> `Channel`{ `ShippingRule` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ShippingRuleApi`** | API context | 
**`rule_id`** | **`String`** |  |
**`shipping_rule_update`** | [**`ShippingRuleUpdate`**](ShippingRuleUpdate.md) |  |

### Return type

[**`ShippingRule`**](ShippingRule.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

