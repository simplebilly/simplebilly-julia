# DeliveryDateApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_delivery_date**](DeliveryDateApi.md#create_delivery_date) | **POST** /api/v1/delivery-dates | 
[**delete_delivery_date**](DeliveryDateApi.md#delete_delivery_date) | **DELETE** /api/v1/delivery-dates/{delivery_date_id} | 
[**get_delivery_date**](DeliveryDateApi.md#get_delivery_date) | **GET** /api/v1/delivery-dates/{delivery_date_id} | 
[**get_delivery_performance**](DeliveryDateApi.md#get_delivery_performance) | **GET** /api/v1/delivery-dates/performance | On-time performance summary: how many promised delivery dates were met within a period.
[**list_delivery_dates**](DeliveryDateApi.md#list_delivery_dates) | **GET** /api/v1/delivery-dates/ | 
[**update_delivery_date**](DeliveryDateApi.md#update_delivery_date) | **PUT** /api/v1/delivery-dates/{delivery_date_id} | 
[**update_delivery_date_status**](DeliveryDateApi.md#update_delivery_date_status) | **PUT** /api/v1/delivery-dates/{delivery_date_id}/status | 


# **create_delivery_date**
> `create_delivery_date`(_api::`DeliveryDateApi`, `delivery_date_create`::`DeliveryDateCreate`; _mediaType=nothing) -> `DeliveryDate`, `OpenAPI.Clients.ApiResponse` <br/>
> `create_delivery_date`(_api::`DeliveryDateApi`, response_stream::`Channel`, `delivery_date_create`::`DeliveryDateCreate`; _mediaType=nothing) -> `Channel`{ `DeliveryDate` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`DeliveryDateApi`** | API context | 
**`delivery_date_create`** | [**`DeliveryDateCreate`**](DeliveryDateCreate.md) |  |

### Return type

[**`DeliveryDate`**](DeliveryDate.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **delete_delivery_date**
> `delete_delivery_date`(_api::`DeliveryDateApi`, `delivery_date_id`::`String`; _mediaType=nothing) -> `Nothing`, `OpenAPI.Clients.ApiResponse` <br/>
> `delete_delivery_date`(_api::`DeliveryDateApi`, response_stream::`Channel`, `delivery_date_id`::`String`; _mediaType=nothing) -> `Channel`{ `Nothing` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`DeliveryDateApi`** | API context | 
**`delivery_date_id`** | **`String`** |  |

### Return type

`Nothing`

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **get_delivery_date**
> `get_delivery_date`(_api::`DeliveryDateApi`, `delivery_date_id`::`String`; _mediaType=nothing) -> `DeliveryDate`, `OpenAPI.Clients.ApiResponse` <br/>
> `get_delivery_date`(_api::`DeliveryDateApi`, response_stream::`Channel`, `delivery_date_id`::`String`; _mediaType=nothing) -> `Channel`{ `DeliveryDate` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`DeliveryDateApi`** | API context | 
**`delivery_date_id`** | **`String`** |  |

### Return type

[**`DeliveryDate`**](DeliveryDate.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **get_delivery_performance**
> `get_delivery_performance`(_api::`DeliveryDateApi`; `page`=nothing, `page_size`=nothing, `order_number`=nothing, `status`=nothing, `from`=nothing, `to`=nothing, _mediaType=nothing) -> `Any`, `OpenAPI.Clients.ApiResponse` <br/>
> `get_delivery_performance`(_api::`DeliveryDateApi`, response_stream::`Channel`; `page`=nothing, `page_size`=nothing, `order_number`=nothing, `status`=nothing, `from`=nothing, `to`=nothing, _mediaType=nothing) -> `Channel`{ `Any` }, `OpenAPI.Clients.ApiResponse`

On-time performance summary: how many promised delivery dates were met within a period.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`DeliveryDateApi`** | API context | 

### Optional Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **`page`** | **`Int64`** |  | [default to nothing]
 **`page_size`** | **`Int64`** |  | [default to nothing]
 **`order_number`** | **`String`** |  | [default to nothing]
 **`status`** | **`String`** |  | [default to nothing]
 **`from`** | **`Date`** | Only dates on or after this date. | [default to nothing]
 **`to`** | **`Date`** | Only dates on or before this date. | [default to nothing]

### Return type

**`Any`**

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **list_delivery_dates**
> `list_delivery_dates`(_api::`DeliveryDateApi`; `page`=nothing, `page_size`=nothing, `order_number`=nothing, `status`=nothing, `from`=nothing, `to`=nothing, _mediaType=nothing) -> `Vector{DeliveryDate}`, `OpenAPI.Clients.ApiResponse` <br/>
> `list_delivery_dates`(_api::`DeliveryDateApi`, response_stream::`Channel`; `page`=nothing, `page_size`=nothing, `order_number`=nothing, `status`=nothing, `from`=nothing, `to`=nothing, _mediaType=nothing) -> `Channel`{ `Vector{DeliveryDate}` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`DeliveryDateApi`** | API context | 

### Optional Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **`page`** | **`Int64`** |  | [default to nothing]
 **`page_size`** | **`Int64`** |  | [default to nothing]
 **`order_number`** | **`String`** |  | [default to nothing]
 **`status`** | **`String`** |  | [default to nothing]
 **`from`** | **`Date`** | Only dates on or after this date. | [default to nothing]
 **`to`** | **`Date`** | Only dates on or before this date. | [default to nothing]

### Return type

[**`Vector{DeliveryDate}`**](DeliveryDate.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **update_delivery_date**
> `update_delivery_date`(_api::`DeliveryDateApi`, `delivery_date_id`::`String`, `body`::`Any`; _mediaType=nothing) -> `DeliveryDate`, `OpenAPI.Clients.ApiResponse` <br/>
> `update_delivery_date`(_api::`DeliveryDateApi`, response_stream::`Channel`, `delivery_date_id`::`String`, `body`::`Any`; _mediaType=nothing) -> `Channel`{ `DeliveryDate` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`DeliveryDateApi`** | API context | 
**`delivery_date_id`** | **`String`** |  |
**`body`** | **`Any`** |  |

### Return type

[**`DeliveryDate`**](DeliveryDate.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **update_delivery_date_status**
> `update_delivery_date_status`(_api::`DeliveryDateApi`, `delivery_date_id`::`String`, `delivery_date_status_update`::`DeliveryDateStatusUpdate`; _mediaType=nothing) -> `DeliveryDate`, `OpenAPI.Clients.ApiResponse` <br/>
> `update_delivery_date_status`(_api::`DeliveryDateApi`, response_stream::`Channel`, `delivery_date_id`::`String`, `delivery_date_status_update`::`DeliveryDateStatusUpdate`; _mediaType=nothing) -> `Channel`{ `DeliveryDate` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`DeliveryDateApi`** | API context | 
**`delivery_date_id`** | **`String`** |  |
**`delivery_date_status_update`** | [**`DeliveryDateStatusUpdate`**](DeliveryDateStatusUpdate.md) |  |

### Return type

[**`DeliveryDate`**](DeliveryDate.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

