# PaymentApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_payment**](PaymentApi.md#create_payment) | **POST** /api/v1/payments | 
[**delete_payment**](PaymentApi.md#delete_payment) | **DELETE** /api/v1/payments/{id} | 
[**get_payment**](PaymentApi.md#get_payment) | **GET** /api/v1/payments/{id} | 
[**get_payments**](PaymentApi.md#get_payments) | **GET** /api/v1/payments/ | 
[**payment_restore**](PaymentApi.md#payment_restore) | **POST** /api/v1/payments/{id}/restore | 
[**update_payment**](PaymentApi.md#update_payment) | **PUT** /api/v1/payments/{id} | 


# **create_payment**
> `create_payment`(_api::`PaymentApi`, `payment_create`::`PaymentCreate`; _mediaType=nothing) -> `Payment`, `OpenAPI.Clients.ApiResponse` <br/>
> `create_payment`(_api::`PaymentApi`, response_stream::`Channel`, `payment_create`::`PaymentCreate`; _mediaType=nothing) -> `Channel`{ `Payment` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`PaymentApi`** | API context | 
**`payment_create`** | [**`PaymentCreate`**](PaymentCreate.md) |  |

### Return type

[**`Payment`**](Payment.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **delete_payment**
> `delete_payment`(_api::`PaymentApi`, `id`::`String`; _mediaType=nothing) -> `Nothing`, `OpenAPI.Clients.ApiResponse` <br/>
> `delete_payment`(_api::`PaymentApi`, response_stream::`Channel`, `id`::`String`; _mediaType=nothing) -> `Channel`{ `Nothing` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`PaymentApi`** | API context | 
**`id`** | **`String`** |  |

### Return type

`Nothing`

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **get_payment**
> `get_payment`(_api::`PaymentApi`, `id`::`String`; _mediaType=nothing) -> `Payment`, `OpenAPI.Clients.ApiResponse` <br/>
> `get_payment`(_api::`PaymentApi`, response_stream::`Channel`, `id`::`String`; _mediaType=nothing) -> `Channel`{ `Payment` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`PaymentApi`** | API context | 
**`id`** | **`String`** |  |

### Return type

[**`Payment`**](Payment.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **get_payments**
> `get_payments`(_api::`PaymentApi`; `page`=nothing, `page_size`=nothing, `search`=nothing, `include_deleted`=nothing, _mediaType=nothing) -> `Vector{Payment}`, `OpenAPI.Clients.ApiResponse` <br/>
> `get_payments`(_api::`PaymentApi`, response_stream::`Channel`; `page`=nothing, `page_size`=nothing, `search`=nothing, `include_deleted`=nothing, _mediaType=nothing) -> `Channel`{ `Vector{Payment}` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`PaymentApi`** | API context | 

### Optional Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **`page`** | **`Int64`** |  | [default to nothing]
 **`page_size`** | **`Int64`** |  | [default to nothing]
 **`search`** | **`String`** |  | [default to nothing]
 **`include_deleted`** | **`Bool`** | Soft-delete entities: set true to include rows with &#x60;deleted_at&#x60; set. | [default to nothing]

### Return type

[**`Vector{Payment}`**](Payment.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **payment_restore**
> `payment_restore`(_api::`PaymentApi`, `id`::`String`; _mediaType=nothing) -> `Payment`, `OpenAPI.Clients.ApiResponse` <br/>
> `payment_restore`(_api::`PaymentApi`, response_stream::`Channel`, `id`::`String`; _mediaType=nothing) -> `Channel`{ `Payment` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`PaymentApi`** | API context | 
**`id`** | **`String`** |  |

### Return type

[**`Payment`**](Payment.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **update_payment**
> `update_payment`(_api::`PaymentApi`, `id`::`String`, `body`::`Any`; _mediaType=nothing) -> `Payment`, `OpenAPI.Clients.ApiResponse` <br/>
> `update_payment`(_api::`PaymentApi`, response_stream::`Channel`, `id`::`String`, `body`::`Any`; _mediaType=nothing) -> `Channel`{ `Payment` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`PaymentApi`** | API context | 
**`id`** | **`String`** |  |
**`body`** | **`Any`** |  |

### Return type

[**`Payment`**](Payment.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

