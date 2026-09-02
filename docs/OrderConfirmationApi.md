# OrderConfirmationApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_confirmation**](OrderConfirmationApi.md#create_confirmation) | **POST** /api/v1/order-confirmations | 
[**delete_confirmation**](OrderConfirmationApi.md#delete_confirmation) | **DELETE** /api/v1/order-confirmations/{confirmation_id} | 
[**download_confirmation_pdf**](OrderConfirmationApi.md#download_confirmation_pdf) | **GET** /api/v1/order-confirmations/{confirmation_id}/pdf | 
[**get_confirmation**](OrderConfirmationApi.md#get_confirmation) | **GET** /api/v1/order-confirmations/{confirmation_id} | 
[**list_confirmations**](OrderConfirmationApi.md#list_confirmations) | **GET** /api/v1/order-confirmations/ | 
[**orderconfirmation_restore**](OrderConfirmationApi.md#orderconfirmation_restore) | **POST** /api/v1/order-confirmations/{confirmation_id}/restore | 
[**pursue_confirmation**](OrderConfirmationApi.md#pursue_confirmation) | **POST** /api/v1/order-confirmations/{confirmation_id}/pursue | 


# **create_confirmation**
> `create_confirmation`(_api::`OrderConfirmationApi`, `order_confirmation_create`::`OrderConfirmationCreate`; _mediaType=nothing) -> `OrderConfirmation`, `OpenAPI.Clients.ApiResponse` <br/>
> `create_confirmation`(_api::`OrderConfirmationApi`, response_stream::`Channel`, `order_confirmation_create`::`OrderConfirmationCreate`; _mediaType=nothing) -> `Channel`{ `OrderConfirmation` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`OrderConfirmationApi`** | API context | 
**`order_confirmation_create`** | [**`OrderConfirmationCreate`**](OrderConfirmationCreate.md) |  |

### Return type

[**`OrderConfirmation`**](OrderConfirmation.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **delete_confirmation**
> `delete_confirmation`(_api::`OrderConfirmationApi`, `confirmation_id`::`String`; _mediaType=nothing) -> `Nothing`, `OpenAPI.Clients.ApiResponse` <br/>
> `delete_confirmation`(_api::`OrderConfirmationApi`, response_stream::`Channel`, `confirmation_id`::`String`; _mediaType=nothing) -> `Channel`{ `Nothing` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`OrderConfirmationApi`** | API context | 
**`confirmation_id`** | **`String`** |  |

### Return type

`Nothing`

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **download_confirmation_pdf**
> `download_confirmation_pdf`(_api::`OrderConfirmationApi`, `confirmation_id`::`String`; _mediaType=nothing) -> `Nothing`, `OpenAPI.Clients.ApiResponse` <br/>
> `download_confirmation_pdf`(_api::`OrderConfirmationApi`, response_stream::`Channel`, `confirmation_id`::`String`; _mediaType=nothing) -> `Channel`{ `Nothing` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`OrderConfirmationApi`** | API context | 
**`confirmation_id`** | **`String`** |  |

### Return type

`Nothing`

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/pdf, application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **get_confirmation**
> `get_confirmation`(_api::`OrderConfirmationApi`, `confirmation_id`::`String`; _mediaType=nothing) -> `OrderConfirmation`, `OpenAPI.Clients.ApiResponse` <br/>
> `get_confirmation`(_api::`OrderConfirmationApi`, response_stream::`Channel`, `confirmation_id`::`String`; _mediaType=nothing) -> `Channel`{ `OrderConfirmation` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`OrderConfirmationApi`** | API context | 
**`confirmation_id`** | **`String`** |  |

### Return type

[**`OrderConfirmation`**](OrderConfirmation.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **list_confirmations**
> `list_confirmations`(_api::`OrderConfirmationApi`; `page`=nothing, `page_size`=nothing, `search`=nothing, `include_deleted`=nothing, _mediaType=nothing) -> `Vector{OrderConfirmation}`, `OpenAPI.Clients.ApiResponse` <br/>
> `list_confirmations`(_api::`OrderConfirmationApi`, response_stream::`Channel`; `page`=nothing, `page_size`=nothing, `search`=nothing, `include_deleted`=nothing, _mediaType=nothing) -> `Channel`{ `Vector{OrderConfirmation}` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`OrderConfirmationApi`** | API context | 

### Optional Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **`page`** | **`Int64`** |  | [default to nothing]
 **`page_size`** | **`Int64`** |  | [default to nothing]
 **`search`** | **`String`** |  | [default to nothing]
 **`include_deleted`** | **`Bool`** | Soft-delete entities: set true to include rows with &#x60;deleted_at&#x60; set. | [default to nothing]

### Return type

[**`Vector{OrderConfirmation}`**](OrderConfirmation.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **orderconfirmation_restore**
> `orderconfirmation_restore`(_api::`OrderConfirmationApi`, `confirmation_id`::`String`; _mediaType=nothing) -> `OrderConfirmation`, `OpenAPI.Clients.ApiResponse` <br/>
> `orderconfirmation_restore`(_api::`OrderConfirmationApi`, response_stream::`Channel`, `confirmation_id`::`String`; _mediaType=nothing) -> `Channel`{ `OrderConfirmation` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`OrderConfirmationApi`** | API context | 
**`confirmation_id`** | **`String`** |  |

### Return type

[**`OrderConfirmation`**](OrderConfirmation.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **pursue_confirmation**
> `pursue_confirmation`(_api::`OrderConfirmationApi`, `confirmation_id`::`String`; _mediaType=nothing) -> `DeliveryNote`, `OpenAPI.Clients.ApiResponse` <br/>
> `pursue_confirmation`(_api::`OrderConfirmationApi`, response_stream::`Channel`, `confirmation_id`::`String`; _mediaType=nothing) -> `Channel`{ `DeliveryNote` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`OrderConfirmationApi`** | API context | 
**`confirmation_id`** | **`String`** |  |

### Return type

[**`DeliveryNote`**](DeliveryNote.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

