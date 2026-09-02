# CustomerGroupApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**add_group_members**](CustomerGroupApi.md#add_group_members) | **POST** /api/v1/customer-groups/{customer_group_id}/members | 
[**create_customer_group**](CustomerGroupApi.md#create_customer_group) | **POST** /api/v1/customer-groups | 
[**delete_customer_group**](CustomerGroupApi.md#delete_customer_group) | **DELETE** /api/v1/customer-groups/{customer_group_id} | 
[**get_customer_group**](CustomerGroupApi.md#get_customer_group) | **GET** /api/v1/customer-groups/{customer_group_id} | 
[**list_customer_groups**](CustomerGroupApi.md#list_customer_groups) | **GET** /api/v1/customer-groups/ | 
[**update_customer_group**](CustomerGroupApi.md#update_customer_group) | **PUT** /api/v1/customer-groups/{customer_group_id} | 


# **add_group_members**
> `add_group_members`(_api::`CustomerGroupApi`, `customer_group_id`::`String`, `body`::`Any`; _mediaType=nothing) -> `CustomerGroup`, `OpenAPI.Clients.ApiResponse` <br/>
> `add_group_members`(_api::`CustomerGroupApi`, response_stream::`Channel`, `customer_group_id`::`String`, `body`::`Any`; _mediaType=nothing) -> `Channel`{ `CustomerGroup` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`CustomerGroupApi`** | API context | 
**`customer_group_id`** | **`String`** |  |
**`body`** | **`Any`** |  |

### Return type

[**`CustomerGroup`**](CustomerGroup.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **create_customer_group**
> `create_customer_group`(_api::`CustomerGroupApi`, `customer_group_create`::`CustomerGroupCreate`; _mediaType=nothing) -> `CustomerGroup`, `OpenAPI.Clients.ApiResponse` <br/>
> `create_customer_group`(_api::`CustomerGroupApi`, response_stream::`Channel`, `customer_group_create`::`CustomerGroupCreate`; _mediaType=nothing) -> `Channel`{ `CustomerGroup` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`CustomerGroupApi`** | API context | 
**`customer_group_create`** | [**`CustomerGroupCreate`**](CustomerGroupCreate.md) |  |

### Return type

[**`CustomerGroup`**](CustomerGroup.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **delete_customer_group**
> `delete_customer_group`(_api::`CustomerGroupApi`, `customer_group_id`::`String`; _mediaType=nothing) -> `Nothing`, `OpenAPI.Clients.ApiResponse` <br/>
> `delete_customer_group`(_api::`CustomerGroupApi`, response_stream::`Channel`, `customer_group_id`::`String`; _mediaType=nothing) -> `Channel`{ `Nothing` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`CustomerGroupApi`** | API context | 
**`customer_group_id`** | **`String`** |  |

### Return type

`Nothing`

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **get_customer_group**
> `get_customer_group`(_api::`CustomerGroupApi`, `customer_group_id`::`String`; _mediaType=nothing) -> `CustomerGroup`, `OpenAPI.Clients.ApiResponse` <br/>
> `get_customer_group`(_api::`CustomerGroupApi`, response_stream::`Channel`, `customer_group_id`::`String`; _mediaType=nothing) -> `Channel`{ `CustomerGroup` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`CustomerGroupApi`** | API context | 
**`customer_group_id`** | **`String`** |  |

### Return type

[**`CustomerGroup`**](CustomerGroup.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **list_customer_groups**
> `list_customer_groups`(_api::`CustomerGroupApi`; `page`=nothing, `page_size`=nothing, `search`=nothing, `include_deleted`=nothing, _mediaType=nothing) -> `Vector{CustomerGroup}`, `OpenAPI.Clients.ApiResponse` <br/>
> `list_customer_groups`(_api::`CustomerGroupApi`, response_stream::`Channel`; `page`=nothing, `page_size`=nothing, `search`=nothing, `include_deleted`=nothing, _mediaType=nothing) -> `Channel`{ `Vector{CustomerGroup}` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`CustomerGroupApi`** | API context | 

### Optional Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **`page`** | **`Int64`** |  | [default to nothing]
 **`page_size`** | **`Int64`** |  | [default to nothing]
 **`search`** | **`String`** |  | [default to nothing]
 **`include_deleted`** | **`Bool`** | Soft-delete entities: set true to include rows with &#x60;deleted_at&#x60; set. | [default to nothing]

### Return type

[**`Vector{CustomerGroup}`**](CustomerGroup.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **update_customer_group**
> `update_customer_group`(_api::`CustomerGroupApi`, `customer_group_id`::`String`, `customer_group_update`::`CustomerGroupUpdate`; _mediaType=nothing) -> `CustomerGroup`, `OpenAPI.Clients.ApiResponse` <br/>
> `update_customer_group`(_api::`CustomerGroupApi`, response_stream::`Channel`, `customer_group_id`::`String`, `customer_group_update`::`CustomerGroupUpdate`; _mediaType=nothing) -> `Channel`{ `CustomerGroup` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`CustomerGroupApi`** | API context | 
**`customer_group_id`** | **`String`** |  |
**`customer_group_update`** | [**`CustomerGroupUpdate`**](CustomerGroupUpdate.md) |  |

### Return type

[**`CustomerGroup`**](CustomerGroup.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

