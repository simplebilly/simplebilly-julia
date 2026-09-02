# GroupFigureApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_group_figure**](GroupFigureApi.md#create_group_figure) | **POST** /api/v1/group-figures | 
[**delete_group_figure**](GroupFigureApi.md#delete_group_figure) | **DELETE** /api/v1/group-figures/{year} | 
[**get_group_figure**](GroupFigureApi.md#get_group_figure) | **GET** /api/v1/group-figures/{year} | 
[**get_group_figures**](GroupFigureApi.md#get_group_figures) | **GET** /api/v1/group-figures/ | 
[**update_group_figure**](GroupFigureApi.md#update_group_figure) | **PUT** /api/v1/group-figures/{year} | 


# **create_group_figure**
> `create_group_figure`(_api::`GroupFigureApi`, `group_figure_create`::`GroupFigureCreate`; _mediaType=nothing) -> `GroupFigure`, `OpenAPI.Clients.ApiResponse` <br/>
> `create_group_figure`(_api::`GroupFigureApi`, response_stream::`Channel`, `group_figure_create`::`GroupFigureCreate`; _mediaType=nothing) -> `Channel`{ `GroupFigure` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`GroupFigureApi`** | API context | 
**`group_figure_create`** | [**`GroupFigureCreate`**](GroupFigureCreate.md) |  |

### Return type

[**`GroupFigure`**](GroupFigure.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **delete_group_figure**
> `delete_group_figure`(_api::`GroupFigureApi`, `year`::`Int64`; _mediaType=nothing) -> `Nothing`, `OpenAPI.Clients.ApiResponse` <br/>
> `delete_group_figure`(_api::`GroupFigureApi`, response_stream::`Channel`, `year`::`Int64`; _mediaType=nothing) -> `Channel`{ `Nothing` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`GroupFigureApi`** | API context | 
**`year`** | **`Int64`** |  |

### Return type

`Nothing`

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **get_group_figure**
> `get_group_figure`(_api::`GroupFigureApi`, `year`::`Int64`; _mediaType=nothing) -> `GroupFigure`, `OpenAPI.Clients.ApiResponse` <br/>
> `get_group_figure`(_api::`GroupFigureApi`, response_stream::`Channel`, `year`::`Int64`; _mediaType=nothing) -> `Channel`{ `GroupFigure` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`GroupFigureApi`** | API context | 
**`year`** | **`Int64`** |  |

### Return type

[**`GroupFigure`**](GroupFigure.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **get_group_figures**
> `get_group_figures`(_api::`GroupFigureApi`; `page`=nothing, `page_size`=nothing, `search`=nothing, `include_deleted`=nothing, _mediaType=nothing) -> `Vector{GroupFigure}`, `OpenAPI.Clients.ApiResponse` <br/>
> `get_group_figures`(_api::`GroupFigureApi`, response_stream::`Channel`; `page`=nothing, `page_size`=nothing, `search`=nothing, `include_deleted`=nothing, _mediaType=nothing) -> `Channel`{ `Vector{GroupFigure}` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`GroupFigureApi`** | API context | 

### Optional Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **`page`** | **`Int64`** |  | [default to nothing]
 **`page_size`** | **`Int64`** |  | [default to nothing]
 **`search`** | **`String`** |  | [default to nothing]
 **`include_deleted`** | **`Bool`** | Soft-delete entities: set true to include rows with &#x60;deleted_at&#x60; set. | [default to nothing]

### Return type

[**`Vector{GroupFigure}`**](GroupFigure.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **update_group_figure**
> `update_group_figure`(_api::`GroupFigureApi`, `year`::`Int64`, `group_figure_update`::`GroupFigureUpdate`; _mediaType=nothing) -> `GroupFigure`, `OpenAPI.Clients.ApiResponse` <br/>
> `update_group_figure`(_api::`GroupFigureApi`, response_stream::`Channel`, `year`::`Int64`, `group_figure_update`::`GroupFigureUpdate`; _mediaType=nothing) -> `Channel`{ `GroupFigure` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`GroupFigureApi`** | API context | 
**`year`** | **`Int64`** |  |
**`group_figure_update`** | [**`GroupFigureUpdate`**](GroupFigureUpdate.md) |  |

### Return type

[**`GroupFigure`**](GroupFigure.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

