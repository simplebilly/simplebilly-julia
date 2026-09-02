# CustomerApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_customer**](CustomerApi.md#create_customer) | **POST** /api/v1/customers | 
[**customer_restore**](CustomerApi.md#customer_restore) | **POST** /api/v1/customers/{customer_id}/restore | 
[**delete_customer**](CustomerApi.md#delete_customer) | **DELETE** /api/v1/customers/{customer_id} | 
[**get_customer**](CustomerApi.md#get_customer) | **GET** /api/v1/customers/{customer_id} | 
[**get_customers**](CustomerApi.md#get_customers) | **GET** /api/v1/customers/ | 
[**update_customer**](CustomerApi.md#update_customer) | **PUT** /api/v1/customers/{customer_id} | 


# **create_customer**
> `create_customer`(_api::`CustomerApi`, `customer_create`::`CustomerCreate`; _mediaType=nothing) -> `Customer`, `OpenAPI.Clients.ApiResponse` <br/>
> `create_customer`(_api::`CustomerApi`, response_stream::`Channel`, `customer_create`::`CustomerCreate`; _mediaType=nothing) -> `Channel`{ `Customer` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`CustomerApi`** | API context | 
**`customer_create`** | [**`CustomerCreate`**](CustomerCreate.md) |  |

### Return type

[**`Customer`**](Customer.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **customer_restore**
> `customer_restore`(_api::`CustomerApi`, `customer_id`::`String`; _mediaType=nothing) -> `Customer`, `OpenAPI.Clients.ApiResponse` <br/>
> `customer_restore`(_api::`CustomerApi`, response_stream::`Channel`, `customer_id`::`String`; _mediaType=nothing) -> `Channel`{ `Customer` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`CustomerApi`** | API context | 
**`customer_id`** | **`String`** |  |

### Return type

[**`Customer`**](Customer.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **delete_customer**
> `delete_customer`(_api::`CustomerApi`, `customer_id`::`String`; _mediaType=nothing) -> `Nothing`, `OpenAPI.Clients.ApiResponse` <br/>
> `delete_customer`(_api::`CustomerApi`, response_stream::`Channel`, `customer_id`::`String`; _mediaType=nothing) -> `Channel`{ `Nothing` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`CustomerApi`** | API context | 
**`customer_id`** | **`String`** |  |

### Return type

`Nothing`

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **get_customer**
> `get_customer`(_api::`CustomerApi`, `customer_id`::`String`; _mediaType=nothing) -> `Customer`, `OpenAPI.Clients.ApiResponse` <br/>
> `get_customer`(_api::`CustomerApi`, response_stream::`Channel`, `customer_id`::`String`; _mediaType=nothing) -> `Channel`{ `Customer` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`CustomerApi`** | API context | 
**`customer_id`** | **`String`** |  |

### Return type

[**`Customer`**](Customer.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **get_customers**
> `get_customers`(_api::`CustomerApi`; `page`=nothing, `page_size`=nothing, `search`=nothing, `include_deleted`=nothing, _mediaType=nothing) -> `Vector{Customer}`, `OpenAPI.Clients.ApiResponse` <br/>
> `get_customers`(_api::`CustomerApi`, response_stream::`Channel`; `page`=nothing, `page_size`=nothing, `search`=nothing, `include_deleted`=nothing, _mediaType=nothing) -> `Channel`{ `Vector{Customer}` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`CustomerApi`** | API context | 

### Optional Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **`page`** | **`Int64`** |  | [default to nothing]
 **`page_size`** | **`Int64`** |  | [default to nothing]
 **`search`** | **`String`** |  | [default to nothing]
 **`include_deleted`** | **`Bool`** | Soft-delete entities: set true to include rows with &#x60;deleted_at&#x60; set. | [default to nothing]

### Return type

[**`Vector{Customer}`**](Customer.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **update_customer**
> `update_customer`(_api::`CustomerApi`, `customer_id`::`String`, `customer_update`::`CustomerUpdate`; _mediaType=nothing) -> `Customer`, `OpenAPI.Clients.ApiResponse` <br/>
> `update_customer`(_api::`CustomerApi`, response_stream::`Channel`, `customer_id`::`String`, `customer_update`::`CustomerUpdate`; _mediaType=nothing) -> `Channel`{ `Customer` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`CustomerApi`** | API context | 
**`customer_id`** | **`String`** |  |
**`customer_update`** | [**`CustomerUpdate`**](CustomerUpdate.md) |  |

### Return type

[**`Customer`**](Customer.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

