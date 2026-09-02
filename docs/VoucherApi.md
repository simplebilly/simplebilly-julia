# VoucherApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_voucher**](VoucherApi.md#create_voucher) | **POST** /api/v1/vouchers | 
[**delete_voucher**](VoucherApi.md#delete_voucher) | **DELETE** /api/v1/vouchers/{voucher_id} | 
[**get_voucher**](VoucherApi.md#get_voucher) | **GET** /api/v1/vouchers/{voucher_id} | 
[**list_vouchers**](VoucherApi.md#list_vouchers) | **GET** /api/v1/vouchers/ | 
[**update_voucher**](VoucherApi.md#update_voucher) | **PUT** /api/v1/vouchers/{voucher_id} | 
[**voucher_restore**](VoucherApi.md#voucher_restore) | **POST** /api/v1/vouchers/{voucher_id}/restore | 


# **create_voucher**
> `create_voucher`(_api::`VoucherApi`, `voucher_create`::`VoucherCreate`; _mediaType=nothing) -> `Voucher`, `OpenAPI.Clients.ApiResponse` <br/>
> `create_voucher`(_api::`VoucherApi`, response_stream::`Channel`, `voucher_create`::`VoucherCreate`; _mediaType=nothing) -> `Channel`{ `Voucher` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`VoucherApi`** | API context | 
**`voucher_create`** | [**`VoucherCreate`**](VoucherCreate.md) |  |

### Return type

[**`Voucher`**](Voucher.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **delete_voucher**
> `delete_voucher`(_api::`VoucherApi`, `voucher_id`::`String`; _mediaType=nothing) -> `Nothing`, `OpenAPI.Clients.ApiResponse` <br/>
> `delete_voucher`(_api::`VoucherApi`, response_stream::`Channel`, `voucher_id`::`String`; _mediaType=nothing) -> `Channel`{ `Nothing` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`VoucherApi`** | API context | 
**`voucher_id`** | **`String`** |  |

### Return type

`Nothing`

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **get_voucher**
> `get_voucher`(_api::`VoucherApi`, `voucher_id`::`String`; _mediaType=nothing) -> `Voucher`, `OpenAPI.Clients.ApiResponse` <br/>
> `get_voucher`(_api::`VoucherApi`, response_stream::`Channel`, `voucher_id`::`String`; _mediaType=nothing) -> `Channel`{ `Voucher` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`VoucherApi`** | API context | 
**`voucher_id`** | **`String`** |  |

### Return type

[**`Voucher`**](Voucher.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **list_vouchers**
> `list_vouchers`(_api::`VoucherApi`; `page`=nothing, `page_size`=nothing, `voucher_type`=nothing, `voucher_status`=nothing, `contact_name`=nothing, `date_from`=nothing, `date_to`=nothing, _mediaType=nothing) -> `Vector{Voucher}`, `OpenAPI.Clients.ApiResponse` <br/>
> `list_vouchers`(_api::`VoucherApi`, response_stream::`Channel`; `page`=nothing, `page_size`=nothing, `voucher_type`=nothing, `voucher_status`=nothing, `contact_name`=nothing, `date_from`=nothing, `date_to`=nothing, _mediaType=nothing) -> `Channel`{ `Vector{Voucher}` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`VoucherApi`** | API context | 

### Optional Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **`page`** | **`Int64`** |  | [default to nothing]
 **`page_size`** | **`Int64`** |  | [default to nothing]
 **`voucher_type`** | **`String`** |  | [default to nothing]
 **`voucher_status`** | **`String`** |  | [default to nothing]
 **`contact_name`** | **`String`** |  | [default to nothing]
 **`date_from`** | **`Date`** |  | [default to nothing]
 **`date_to`** | **`Date`** |  | [default to nothing]

### Return type

[**`Vector{Voucher}`**](Voucher.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **update_voucher**
> `update_voucher`(_api::`VoucherApi`, `voucher_id`::`String`, `body`::`Any`; _mediaType=nothing) -> `Voucher`, `OpenAPI.Clients.ApiResponse` <br/>
> `update_voucher`(_api::`VoucherApi`, response_stream::`Channel`, `voucher_id`::`String`, `body`::`Any`; _mediaType=nothing) -> `Channel`{ `Voucher` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`VoucherApi`** | API context | 
**`voucher_id`** | **`String`** |  |
**`body`** | **`Any`** |  |

### Return type

[**`Voucher`**](Voucher.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **voucher_restore**
> `voucher_restore`(_api::`VoucherApi`, `voucher_id`::`String`; _mediaType=nothing) -> `Voucher`, `OpenAPI.Clients.ApiResponse` <br/>
> `voucher_restore`(_api::`VoucherApi`, response_stream::`Channel`, `voucher_id`::`String`; _mediaType=nothing) -> `Channel`{ `Voucher` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`VoucherApi`** | API context | 
**`voucher_id`** | **`String`** |  |

### Return type

[**`Voucher`**](Voucher.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

