# PaymentGatewayApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_payment_gateway_api**](PaymentGatewayApi.md#create_payment_gateway_api) | **POST** /api/v1/payment-gateways | 
[**delete_payment_gateway_api**](PaymentGatewayApi.md#delete_payment_gateway_api) | **DELETE** /api/v1/payment-gateways/{gateway_id} | 
[**list_payment_gateways_api**](PaymentGatewayApi.md#list_payment_gateways_api) | **GET** /api/v1/payment-gateways/ | 
[**oauth_authorize_api**](PaymentGatewayApi.md#oauth_authorize_api) | **POST** /api/v1/payment-gateways/oauth/authorize | 
[**oauth_callback_api**](PaymentGatewayApi.md#oauth_callback_api) | **POST** /api/v1/payment-gateways/oauth/callback | 
[**update_payment_gateway_api**](PaymentGatewayApi.md#update_payment_gateway_api) | **PUT** /api/v1/payment-gateways/{gateway_id} | 


# **create_payment_gateway_api**
> `create_payment_gateway_api`(_api::`PaymentGatewayApi`, `body`::`Any`; _mediaType=nothing) -> `PaymentGateway`, `OpenAPI.Clients.ApiResponse` <br/>
> `create_payment_gateway_api`(_api::`PaymentGatewayApi`, response_stream::`Channel`, `body`::`Any`; _mediaType=nothing) -> `Channel`{ `PaymentGateway` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`PaymentGatewayApi`** | API context | 
**`body`** | **`Any`** |  |

### Return type

[**`PaymentGateway`**](PaymentGateway.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **delete_payment_gateway_api**
> `delete_payment_gateway_api`(_api::`PaymentGatewayApi`, `gateway_id`::`String`; _mediaType=nothing) -> `Nothing`, `OpenAPI.Clients.ApiResponse` <br/>
> `delete_payment_gateway_api`(_api::`PaymentGatewayApi`, response_stream::`Channel`, `gateway_id`::`String`; _mediaType=nothing) -> `Channel`{ `Nothing` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`PaymentGatewayApi`** | API context | 
**`gateway_id`** | **`String`** |  |

### Return type

`Nothing`

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **list_payment_gateways_api**
> `list_payment_gateways_api`(_api::`PaymentGatewayApi`; _mediaType=nothing) -> `Vector{PaymentGateway}`, `OpenAPI.Clients.ApiResponse` <br/>
> `list_payment_gateways_api`(_api::`PaymentGatewayApi`, response_stream::`Channel`; _mediaType=nothing) -> `Channel`{ `Vector{PaymentGateway}` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters
This endpoint does not need any parameter.

### Return type

[**`Vector{PaymentGateway}`**](PaymentGateway.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **oauth_authorize_api**
> `oauth_authorize_api`(_api::`PaymentGatewayApi`, `gateway_o_auth_authorize_request`::`GatewayOAuthAuthorizeRequest`; _mediaType=nothing) -> `GatewayOAuthAuthorizeResponse`, `OpenAPI.Clients.ApiResponse` <br/>
> `oauth_authorize_api`(_api::`PaymentGatewayApi`, response_stream::`Channel`, `gateway_o_auth_authorize_request`::`GatewayOAuthAuthorizeRequest`; _mediaType=nothing) -> `Channel`{ `GatewayOAuthAuthorizeResponse` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`PaymentGatewayApi`** | API context | 
**`gateway_o_auth_authorize_request`** | [**`GatewayOAuthAuthorizeRequest`**](GatewayOAuthAuthorizeRequest.md) |  |

### Return type

[**`GatewayOAuthAuthorizeResponse`**](GatewayOAuthAuthorizeResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **oauth_callback_api**
> `oauth_callback_api`(_api::`PaymentGatewayApi`, `gateway_o_auth_callback_request`::`GatewayOAuthCallbackRequest`; _mediaType=nothing) -> `PaymentGateway`, `OpenAPI.Clients.ApiResponse` <br/>
> `oauth_callback_api`(_api::`PaymentGatewayApi`, response_stream::`Channel`, `gateway_o_auth_callback_request`::`GatewayOAuthCallbackRequest`; _mediaType=nothing) -> `Channel`{ `PaymentGateway` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`PaymentGatewayApi`** | API context | 
**`gateway_o_auth_callback_request`** | [**`GatewayOAuthCallbackRequest`**](GatewayOAuthCallbackRequest.md) |  |

### Return type

[**`PaymentGateway`**](PaymentGateway.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **update_payment_gateway_api**
> `update_payment_gateway_api`(_api::`PaymentGatewayApi`, `gateway_id`::`String`, `body`::`Any`; _mediaType=nothing) -> `PaymentGateway`, `OpenAPI.Clients.ApiResponse` <br/>
> `update_payment_gateway_api`(_api::`PaymentGatewayApi`, response_stream::`Channel`, `gateway_id`::`String`, `body`::`Any`; _mediaType=nothing) -> `Channel`{ `PaymentGateway` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`PaymentGatewayApi`** | API context | 
**`gateway_id`** | **`String`** |  |
**`body`** | **`Any`** |  |

### Return type

[**`PaymentGateway`**](PaymentGateway.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

