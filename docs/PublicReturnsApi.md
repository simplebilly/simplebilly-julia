# PublicReturnsApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_public_return_status**](PublicReturnsApi.md#get_public_return_status) | **GET** /api/v1/public/returns/status | Customer checks the status of a return (public, no auth). The return is only revealed when its linked order&#39;s email matches.
[**list_public_returns**](PublicReturnsApi.md#list_public_returns) | **GET** /api/v1/public/returns/list | List all returns for an order (public, no auth).
[**request_public_return**](PublicReturnsApi.md#request_public_return) | **POST** /api/v1/public/returns/request | Customer requests a return for an order (public, no auth).


# **get_public_return_status**
> `get_public_return_status`(_api::`PublicReturnsApi`, `email`::`String`; `return_number`=nothing, `return_order_id`=nothing, `order_number`=nothing, _mediaType=nothing) -> `PublicReturnStatusResponse`, `OpenAPI.Clients.ApiResponse` <br/>
> `get_public_return_status`(_api::`PublicReturnsApi`, response_stream::`Channel`, `email`::`String`; `return_number`=nothing, `return_order_id`=nothing, `order_number`=nothing, _mediaType=nothing) -> `Channel`{ `PublicReturnStatusResponse` }, `OpenAPI.Clients.ApiResponse`

Customer checks the status of a return (public, no auth). The return is only revealed when its linked order's email matches.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`PublicReturnsApi`** | API context | 
**`email`** | **`String`** |  |

### Optional Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **`return_number`** | **`String`** | Either return_number or return_order_id must be provided. | [default to nothing]
 **`return_order_id`** | **`String`** |  | [default to nothing]
 **`order_number`** | **`String`** |  | [default to nothing]

### Return type

[**`PublicReturnStatusResponse`**](PublicReturnStatusResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **list_public_returns**
> `list_public_returns`(_api::`PublicReturnsApi`, `order_number`::`String`, `email`::`String`; _mediaType=nothing) -> `Vector{PublicReturnStatusResponse}`, `OpenAPI.Clients.ApiResponse` <br/>
> `list_public_returns`(_api::`PublicReturnsApi`, response_stream::`Channel`, `order_number`::`String`, `email`::`String`; _mediaType=nothing) -> `Channel`{ `Vector{PublicReturnStatusResponse}` }, `OpenAPI.Clients.ApiResponse`

List all returns for an order (public, no auth).

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`PublicReturnsApi`** | API context | 
**`order_number`** | **`String`** |  |
**`email`** | **`String`** |  |

### Return type

[**`Vector{PublicReturnStatusResponse}`**](PublicReturnStatusResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **request_public_return**
> `request_public_return`(_api::`PublicReturnsApi`, `public_return_request`::`PublicReturnRequest`; _mediaType=nothing) -> `PublicReturnResponse`, `OpenAPI.Clients.ApiResponse` <br/>
> `request_public_return`(_api::`PublicReturnsApi`, response_stream::`Channel`, `public_return_request`::`PublicReturnRequest`; _mediaType=nothing) -> `Channel`{ `PublicReturnResponse` }, `OpenAPI.Clients.ApiResponse`

Customer requests a return for an order (public, no auth).

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`PublicReturnsApi`** | API context | 
**`public_return_request`** | [**`PublicReturnRequest`**](PublicReturnRequest.md) |  |

### Return type

[**`PublicReturnResponse`**](PublicReturnResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

