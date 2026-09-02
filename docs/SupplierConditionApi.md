# SupplierConditionApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_supplier_condition**](SupplierConditionApi.md#create_supplier_condition) | **POST** /api/v1/supplier-conditions | 
[**delete_supplier_condition**](SupplierConditionApi.md#delete_supplier_condition) | **DELETE** /api/v1/supplier-conditions/{supplier_condition_id} | 
[**get_supplier_condition**](SupplierConditionApi.md#get_supplier_condition) | **GET** /api/v1/supplier-conditions/{supplier_condition_id} | 
[**list_supplier_conditions**](SupplierConditionApi.md#list_supplier_conditions) | **GET** /api/v1/supplier-conditions/ | 
[**update_supplier_condition**](SupplierConditionApi.md#update_supplier_condition) | **PUT** /api/v1/supplier-conditions/{supplier_condition_id} | 


# **create_supplier_condition**
> `create_supplier_condition`(_api::`SupplierConditionApi`, `supplier_condition_create`::`SupplierConditionCreate`; _mediaType=nothing) -> `SupplierCondition`, `OpenAPI.Clients.ApiResponse` <br/>
> `create_supplier_condition`(_api::`SupplierConditionApi`, response_stream::`Channel`, `supplier_condition_create`::`SupplierConditionCreate`; _mediaType=nothing) -> `Channel`{ `SupplierCondition` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`SupplierConditionApi`** | API context | 
**`supplier_condition_create`** | [**`SupplierConditionCreate`**](SupplierConditionCreate.md) |  |

### Return type

[**`SupplierCondition`**](SupplierCondition.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **delete_supplier_condition**
> `delete_supplier_condition`(_api::`SupplierConditionApi`, `supplier_condition_id`::`String`; _mediaType=nothing) -> `Nothing`, `OpenAPI.Clients.ApiResponse` <br/>
> `delete_supplier_condition`(_api::`SupplierConditionApi`, response_stream::`Channel`, `supplier_condition_id`::`String`; _mediaType=nothing) -> `Channel`{ `Nothing` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`SupplierConditionApi`** | API context | 
**`supplier_condition_id`** | **`String`** |  |

### Return type

`Nothing`

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **get_supplier_condition**
> `get_supplier_condition`(_api::`SupplierConditionApi`, `supplier_condition_id`::`String`; _mediaType=nothing) -> `SupplierCondition`, `OpenAPI.Clients.ApiResponse` <br/>
> `get_supplier_condition`(_api::`SupplierConditionApi`, response_stream::`Channel`, `supplier_condition_id`::`String`; _mediaType=nothing) -> `Channel`{ `SupplierCondition` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`SupplierConditionApi`** | API context | 
**`supplier_condition_id`** | **`String`** |  |

### Return type

[**`SupplierCondition`**](SupplierCondition.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **list_supplier_conditions**
> `list_supplier_conditions`(_api::`SupplierConditionApi`; `page`=nothing, `page_size`=nothing, `supplier_contact_id`=nothing, `search`=nothing, _mediaType=nothing) -> `Vector{SupplierCondition}`, `OpenAPI.Clients.ApiResponse` <br/>
> `list_supplier_conditions`(_api::`SupplierConditionApi`, response_stream::`Channel`; `page`=nothing, `page_size`=nothing, `supplier_contact_id`=nothing, `search`=nothing, _mediaType=nothing) -> `Channel`{ `Vector{SupplierCondition}` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`SupplierConditionApi`** | API context | 

### Optional Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **`page`** | **`Int64`** |  | [default to nothing]
 **`page_size`** | **`Int64`** |  | [default to nothing]
 **`supplier_contact_id`** | **`String`** |  | [default to nothing]
 **`search`** | **`String`** |  | [default to nothing]

### Return type

[**`Vector{SupplierCondition}`**](SupplierCondition.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **update_supplier_condition**
> `update_supplier_condition`(_api::`SupplierConditionApi`, `supplier_condition_id`::`String`, `supplier_condition_update`::`SupplierConditionUpdate`; _mediaType=nothing) -> `SupplierCondition`, `OpenAPI.Clients.ApiResponse` <br/>
> `update_supplier_condition`(_api::`SupplierConditionApi`, response_stream::`Channel`, `supplier_condition_id`::`String`, `supplier_condition_update`::`SupplierConditionUpdate`; _mediaType=nothing) -> `Channel`{ `SupplierCondition` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`SupplierConditionApi`** | API context | 
**`supplier_condition_id`** | **`String`** |  |
**`supplier_condition_update`** | [**`SupplierConditionUpdate`**](SupplierConditionUpdate.md) |  |

### Return type

[**`SupplierCondition`**](SupplierCondition.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

