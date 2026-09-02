# PosApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**pos_billing**](PosApi.md#pos_billing) | **GET** /api/pos/billing | 
[**pos_create_order**](PosApi.md#pos_create_order) | **POST** /api/pos/orders | 
[**pos_create_register**](PosApi.md#pos_create_register) | **POST** /api/pos/registers | 
[**pos_create_table**](PosApi.md#pos_create_table) | **POST** /api/pos/tables | 
[**pos_disable_register**](PosApi.md#pos_disable_register) | **POST** /api/pos/registers/{id}/disable | 
[**pos_free_table**](PosApi.md#pos_free_table) | **POST** /api/pos/tables/{id}/free | 
[**pos_kasse_closing**](PosApi.md#pos_kasse_closing) | **POST** /api/pos/kasse/closing | 
[**pos_kasse_entries**](PosApi.md#pos_kasse_entries) | **GET** /api/pos/kasse/entries | 
[**pos_kasse_export**](PosApi.md#pos_kasse_export) | **GET** /api/pos/kasse/export | 
[**pos_kasse_pay_in_out**](PosApi.md#pos_kasse_pay_in_out) | **POST** /api/pos/kasse/pay-in-out | 
[**pos_list_orders**](PosApi.md#pos_list_orders) | **GET** /api/pos/orders | 
[**pos_list_products**](PosApi.md#pos_list_products) | **GET** /api/pos/products | 
[**pos_list_registers**](PosApi.md#pos_list_registers) | **GET** /api/pos/registers | 
[**pos_list_tables**](PosApi.md#pos_list_tables) | **GET** /api/pos/tables | 
[**pos_order_print**](PosApi.md#pos_order_print) | **GET** /api/pos/orders/{order_number}/print | 
[**pos_order_receipt**](PosApi.md#pos_order_receipt) | **GET** /api/pos/orders/{order_number}/receipt | 
[**pos_pay_order**](PosApi.md#pos_pay_order) | **POST** /api/pos/orders/{order_number}/pay | 
[**pos_sumup_checkout**](PosApi.md#pos_sumup_checkout) | **POST** /api/pos/sumup/checkout | 


# **pos_billing**
> `pos_billing`(_api::`PosApi`; _mediaType=nothing) -> `Any`, `OpenAPI.Clients.ApiResponse` <br/>
> `pos_billing`(_api::`PosApi`, response_stream::`Channel`; _mediaType=nothing) -> `Channel`{ `Any` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters
This endpoint does not need any parameter.

### Return type

**`Any`**

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **pos_create_order**
> `pos_create_order`(_api::`PosApi`, `body`::`Any`; _mediaType=nothing) -> `Any`, `OpenAPI.Clients.ApiResponse` <br/>
> `pos_create_order`(_api::`PosApi`, response_stream::`Channel`, `body`::`Any`; _mediaType=nothing) -> `Channel`{ `Any` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`PosApi`** | API context | 
**`body`** | **`Any`** |  |

### Return type

**`Any`**

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **pos_create_register**
> `pos_create_register`(_api::`PosApi`, `pos_register_create`::`PosRegisterCreate`; _mediaType=nothing) -> `PosRegister`, `OpenAPI.Clients.ApiResponse` <br/>
> `pos_create_register`(_api::`PosApi`, response_stream::`Channel`, `pos_register_create`::`PosRegisterCreate`; _mediaType=nothing) -> `Channel`{ `PosRegister` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`PosApi`** | API context | 
**`pos_register_create`** | [**`PosRegisterCreate`**](PosRegisterCreate.md) |  |

### Return type

[**`PosRegister`**](PosRegister.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **pos_create_table**
> `pos_create_table`(_api::`PosApi`, `pos_table_create`::`PosTableCreate`; _mediaType=nothing) -> `PosTable`, `OpenAPI.Clients.ApiResponse` <br/>
> `pos_create_table`(_api::`PosApi`, response_stream::`Channel`, `pos_table_create`::`PosTableCreate`; _mediaType=nothing) -> `Channel`{ `PosTable` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`PosApi`** | API context | 
**`pos_table_create`** | [**`PosTableCreate`**](PosTableCreate.md) |  |

### Return type

[**`PosTable`**](PosTable.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **pos_disable_register**
> `pos_disable_register`(_api::`PosApi`, `id`::`String`; _mediaType=nothing) -> `PosRegister`, `OpenAPI.Clients.ApiResponse` <br/>
> `pos_disable_register`(_api::`PosApi`, response_stream::`Channel`, `id`::`String`; _mediaType=nothing) -> `Channel`{ `PosRegister` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`PosApi`** | API context | 
**`id`** | **`String`** |  |

### Return type

[**`PosRegister`**](PosRegister.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **pos_free_table**
> `pos_free_table`(_api::`PosApi`, `id`::`String`; _mediaType=nothing) -> `PosTable`, `OpenAPI.Clients.ApiResponse` <br/>
> `pos_free_table`(_api::`PosApi`, response_stream::`Channel`, `id`::`String`; _mediaType=nothing) -> `Channel`{ `PosTable` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`PosApi`** | API context | 
**`id`** | **`String`** |  |

### Return type

[**`PosTable`**](PosTable.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **pos_kasse_closing**
> `pos_kasse_closing`(_api::`PosApi`, `body`::`Any`; _mediaType=nothing) -> `Any`, `OpenAPI.Clients.ApiResponse` <br/>
> `pos_kasse_closing`(_api::`PosApi`, response_stream::`Channel`, `body`::`Any`; _mediaType=nothing) -> `Channel`{ `Any` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`PosApi`** | API context | 
**`body`** | **`Any`** |  |

### Return type

**`Any`**

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **pos_kasse_entries**
> `pos_kasse_entries`(_api::`PosApi`; _mediaType=nothing) -> `Any`, `OpenAPI.Clients.ApiResponse` <br/>
> `pos_kasse_entries`(_api::`PosApi`, response_stream::`Channel`; _mediaType=nothing) -> `Channel`{ `Any` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters
This endpoint does not need any parameter.

### Return type

**`Any`**

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **pos_kasse_export**
> `pos_kasse_export`(_api::`PosApi`; _mediaType=nothing) -> `Any`, `OpenAPI.Clients.ApiResponse` <br/>
> `pos_kasse_export`(_api::`PosApi`, response_stream::`Channel`; _mediaType=nothing) -> `Channel`{ `Any` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters
This endpoint does not need any parameter.

### Return type

**`Any`**

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **pos_kasse_pay_in_out**
> `pos_kasse_pay_in_out`(_api::`PosApi`, `body`::`Any`; _mediaType=nothing) -> `Any`, `OpenAPI.Clients.ApiResponse` <br/>
> `pos_kasse_pay_in_out`(_api::`PosApi`, response_stream::`Channel`, `body`::`Any`; _mediaType=nothing) -> `Channel`{ `Any` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`PosApi`** | API context | 
**`body`** | **`Any`** |  |

### Return type

**`Any`**

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **pos_list_orders**
> `pos_list_orders`(_api::`PosApi`; `status`=nothing, _mediaType=nothing) -> `Any`, `OpenAPI.Clients.ApiResponse` <br/>
> `pos_list_orders`(_api::`PosApi`, response_stream::`Channel`; `status`=nothing, _mediaType=nothing) -> `Channel`{ `Any` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`PosApi`** | API context | 

### Optional Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **`status`** | **`String`** | Filter by order status | [default to nothing]

### Return type

**`Any`**

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **pos_list_products**
> `pos_list_products`(_api::`PosApi`; `q`=nothing, _mediaType=nothing) -> `Any`, `OpenAPI.Clients.ApiResponse` <br/>
> `pos_list_products`(_api::`PosApi`, response_stream::`Channel`; `q`=nothing, _mediaType=nothing) -> `Channel`{ `Any` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`PosApi`** | API context | 

### Optional Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **`q`** | **`String`** | Product search | [default to nothing]

### Return type

**`Any`**

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **pos_list_registers**
> `pos_list_registers`(_api::`PosApi`; _mediaType=nothing) -> `Vector{PosRegister}`, `OpenAPI.Clients.ApiResponse` <br/>
> `pos_list_registers`(_api::`PosApi`, response_stream::`Channel`; _mediaType=nothing) -> `Channel`{ `Vector{PosRegister}` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters
This endpoint does not need any parameter.

### Return type

[**`Vector{PosRegister}`**](PosRegister.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **pos_list_tables**
> `pos_list_tables`(_api::`PosApi`; _mediaType=nothing) -> `Vector{PosTable}`, `OpenAPI.Clients.ApiResponse` <br/>
> `pos_list_tables`(_api::`PosApi`, response_stream::`Channel`; _mediaType=nothing) -> `Channel`{ `Vector{PosTable}` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters
This endpoint does not need any parameter.

### Return type

[**`Vector{PosTable}`**](PosTable.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **pos_order_print**
> `pos_order_print`(_api::`PosApi`, `order_number`::`String`; _mediaType=nothing) -> `Any`, `OpenAPI.Clients.ApiResponse` <br/>
> `pos_order_print`(_api::`PosApi`, response_stream::`Channel`, `order_number`::`String`; _mediaType=nothing) -> `Channel`{ `Any` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`PosApi`** | API context | 
**`order_number`** | **`String`** |  |

### Return type

**`Any`**

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **pos_order_receipt**
> `pos_order_receipt`(_api::`PosApi`, `order_number`::`String`; _mediaType=nothing) -> `Any`, `OpenAPI.Clients.ApiResponse` <br/>
> `pos_order_receipt`(_api::`PosApi`, response_stream::`Channel`, `order_number`::`String`; _mediaType=nothing) -> `Channel`{ `Any` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`PosApi`** | API context | 
**`order_number`** | **`String`** |  |

### Return type

**`Any`**

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **pos_pay_order**
> `pos_pay_order`(_api::`PosApi`, `order_number`::`String`, `body`::`Any`; _mediaType=nothing) -> `Any`, `OpenAPI.Clients.ApiResponse` <br/>
> `pos_pay_order`(_api::`PosApi`, response_stream::`Channel`, `order_number`::`String`, `body`::`Any`; _mediaType=nothing) -> `Channel`{ `Any` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`PosApi`** | API context | 
**`order_number`** | **`String`** |  |
**`body`** | **`Any`** |  |

### Return type

**`Any`**

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **pos_sumup_checkout**
> `pos_sumup_checkout`(_api::`PosApi`, `body`::`Any`; _mediaType=nothing) -> `Any`, `OpenAPI.Clients.ApiResponse` <br/>
> `pos_sumup_checkout`(_api::`PosApi`, response_stream::`Channel`, `body`::`Any`; _mediaType=nothing) -> `Channel`{ `Any` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`PosApi`** | API context | 
**`body`** | **`Any`** |  |

### Return type

**`Any`**

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

