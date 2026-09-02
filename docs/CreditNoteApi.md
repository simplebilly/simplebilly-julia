# CreditNoteApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_credit_note**](CreditNoteApi.md#create_credit_note) | **POST** /api/v1/credit-notes | 
[**download_credit_note_pdf**](CreditNoteApi.md#download_credit_note_pdf) | **GET** /api/v1/credit-notes/{credit_note_id}/pdf | 
[**get_credit_note**](CreditNoteApi.md#get_credit_note) | **GET** /api/v1/credit-notes/{credit_note_id} | 
[**list_credit_notes**](CreditNoteApi.md#list_credit_notes) | **GET** /api/v1/credit-notes/ | 


# **create_credit_note**
> `create_credit_note`(_api::`CreditNoteApi`, `body`::`Any`; _mediaType=nothing) -> `Invoice`, `OpenAPI.Clients.ApiResponse` <br/>
> `create_credit_note`(_api::`CreditNoteApi`, response_stream::`Channel`, `body`::`Any`; _mediaType=nothing) -> `Channel`{ `Invoice` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`CreditNoteApi`** | API context | 
**`body`** | **`Any`** |  |

### Return type

[**`Invoice`**](Invoice.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **download_credit_note_pdf**
> `download_credit_note_pdf`(_api::`CreditNoteApi`, `credit_note_id`::`String`; _mediaType=nothing) -> `Nothing`, `OpenAPI.Clients.ApiResponse` <br/>
> `download_credit_note_pdf`(_api::`CreditNoteApi`, response_stream::`Channel`, `credit_note_id`::`String`; _mediaType=nothing) -> `Channel`{ `Nothing` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`CreditNoteApi`** | API context | 
**`credit_note_id`** | **`String`** |  |

### Return type

`Nothing`

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/pdf, application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **get_credit_note**
> `get_credit_note`(_api::`CreditNoteApi`, `credit_note_id`::`String`; _mediaType=nothing) -> `Invoice`, `OpenAPI.Clients.ApiResponse` <br/>
> `get_credit_note`(_api::`CreditNoteApi`, response_stream::`Channel`, `credit_note_id`::`String`; _mediaType=nothing) -> `Channel`{ `Invoice` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`CreditNoteApi`** | API context | 
**`credit_note_id`** | **`String`** |  |

### Return type

[**`Invoice`**](Invoice.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **list_credit_notes**
> `list_credit_notes`(_api::`CreditNoteApi`; `page`=nothing, `page_size`=nothing, `search`=nothing, `include_deleted`=nothing, _mediaType=nothing) -> `Vector{Invoice}`, `OpenAPI.Clients.ApiResponse` <br/>
> `list_credit_notes`(_api::`CreditNoteApi`, response_stream::`Channel`; `page`=nothing, `page_size`=nothing, `search`=nothing, `include_deleted`=nothing, _mediaType=nothing) -> `Channel`{ `Vector{Invoice}` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`CreditNoteApi`** | API context | 

### Optional Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **`page`** | **`Int64`** |  | [default to nothing]
 **`page_size`** | **`Int64`** |  | [default to nothing]
 **`search`** | **`String`** |  | [default to nothing]
 **`include_deleted`** | **`Bool`** | Soft-delete entities: set true to include rows with &#x60;deleted_at&#x60; set. | [default to nothing]

### Return type

[**`Vector{Invoice}`**](Invoice.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

