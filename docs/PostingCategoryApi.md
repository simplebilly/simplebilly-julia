# PostingCategoryApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_posting_category**](PostingCategoryApi.md#create_posting_category) | **POST** /api/v1/posting-categories | 
[**delete_posting_category**](PostingCategoryApi.md#delete_posting_category) | **DELETE** /api/v1/posting-categories/{category_id} | 
[**list_posting_categories**](PostingCategoryApi.md#list_posting_categories) | **GET** /api/v1/posting-categories | 
[**seed_posting_categories**](PostingCategoryApi.md#seed_posting_categories) | **POST** /api/v1/posting-categories/seed/{skr_version} | 
[**update_posting_category**](PostingCategoryApi.md#update_posting_category) | **PUT** /api/v1/posting-categories/{category_id} | 


# **create_posting_category**
> `create_posting_category`(_api::`PostingCategoryApi`, `body`::`Any`; _mediaType=nothing) -> `PostingCategory`, `OpenAPI.Clients.ApiResponse` <br/>
> `create_posting_category`(_api::`PostingCategoryApi`, response_stream::`Channel`, `body`::`Any`; _mediaType=nothing) -> `Channel`{ `PostingCategory` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`PostingCategoryApi`** | API context | 
**`body`** | **`Any`** |  |

### Return type

[**`PostingCategory`**](PostingCategory.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **delete_posting_category**
> `delete_posting_category`(_api::`PostingCategoryApi`, `category_id`::`String`; _mediaType=nothing) -> `Nothing`, `OpenAPI.Clients.ApiResponse` <br/>
> `delete_posting_category`(_api::`PostingCategoryApi`, response_stream::`Channel`, `category_id`::`String`; _mediaType=nothing) -> `Channel`{ `Nothing` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`PostingCategoryApi`** | API context | 
**`category_id`** | **`String`** |  |

### Return type

`Nothing`

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **list_posting_categories**
> `list_posting_categories`(_api::`PostingCategoryApi`; _mediaType=nothing) -> `Vector{PostingCategory}`, `OpenAPI.Clients.ApiResponse` <br/>
> `list_posting_categories`(_api::`PostingCategoryApi`, response_stream::`Channel`; _mediaType=nothing) -> `Channel`{ `Vector{PostingCategory}` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters
This endpoint does not need any parameter.

### Return type

[**`Vector{PostingCategory}`**](PostingCategory.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **seed_posting_categories**
> `seed_posting_categories`(_api::`PostingCategoryApi`, `skr_version`::`String`; _mediaType=nothing) -> `Nothing`, `OpenAPI.Clients.ApiResponse` <br/>
> `seed_posting_categories`(_api::`PostingCategoryApi`, response_stream::`Channel`, `skr_version`::`String`; _mediaType=nothing) -> `Channel`{ `Nothing` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`PostingCategoryApi`** | API context | 
**`skr_version`** | **`String`** |  |

### Return type

`Nothing`

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **update_posting_category**
> `update_posting_category`(_api::`PostingCategoryApi`, `category_id`::`String`, `body`::`Any`; _mediaType=nothing) -> `PostingCategory`, `OpenAPI.Clients.ApiResponse` <br/>
> `update_posting_category`(_api::`PostingCategoryApi`, response_stream::`Channel`, `category_id`::`String`, `body`::`Any`; _mediaType=nothing) -> `Channel`{ `PostingCategory` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`PostingCategoryApi`** | API context | 
**`category_id`** | **`String`** |  |
**`body`** | **`Any`** |  |

### Return type

[**`PostingCategory`**](PostingCategory.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

