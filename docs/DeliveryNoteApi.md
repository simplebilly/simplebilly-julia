# DeliveryNoteApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_delivery_note**](DeliveryNoteApi.md#create_delivery_note) | **POST** /api/v1/delivery-notes | 
[**delete_delivery_note**](DeliveryNoteApi.md#delete_delivery_note) | **DELETE** /api/v1/delivery-notes/{delivery_note_id} | 
[**deliverynote_restore**](DeliveryNoteApi.md#deliverynote_restore) | **POST** /api/v1/delivery-notes/{delivery_note_id}/restore | 
[**download_delivery_note_pdf**](DeliveryNoteApi.md#download_delivery_note_pdf) | **GET** /api/v1/delivery-notes/{delivery_note_id}/pdf | 
[**get_delivery_note**](DeliveryNoteApi.md#get_delivery_note) | **GET** /api/v1/delivery-notes/{delivery_note_id} | 
[**list_delivery_notes**](DeliveryNoteApi.md#list_delivery_notes) | **GET** /api/v1/delivery-notes/ | 
[**pursue_delivery_note**](DeliveryNoteApi.md#pursue_delivery_note) | **POST** /api/v1/delivery-notes/{delivery_note_id}/pursue | 


# **create_delivery_note**
> `create_delivery_note`(_api::`DeliveryNoteApi`, `delivery_note_create`::`DeliveryNoteCreate`; _mediaType=nothing) -> `DeliveryNote`, `OpenAPI.Clients.ApiResponse` <br/>
> `create_delivery_note`(_api::`DeliveryNoteApi`, response_stream::`Channel`, `delivery_note_create`::`DeliveryNoteCreate`; _mediaType=nothing) -> `Channel`{ `DeliveryNote` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`DeliveryNoteApi`** | API context | 
**`delivery_note_create`** | [**`DeliveryNoteCreate`**](DeliveryNoteCreate.md) |  |

### Return type

[**`DeliveryNote`**](DeliveryNote.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **delete_delivery_note**
> `delete_delivery_note`(_api::`DeliveryNoteApi`, `delivery_note_id`::`String`; _mediaType=nothing) -> `Nothing`, `OpenAPI.Clients.ApiResponse` <br/>
> `delete_delivery_note`(_api::`DeliveryNoteApi`, response_stream::`Channel`, `delivery_note_id`::`String`; _mediaType=nothing) -> `Channel`{ `Nothing` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`DeliveryNoteApi`** | API context | 
**`delivery_note_id`** | **`String`** |  |

### Return type

`Nothing`

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **deliverynote_restore**
> `deliverynote_restore`(_api::`DeliveryNoteApi`, `delivery_note_id`::`String`; _mediaType=nothing) -> `DeliveryNote`, `OpenAPI.Clients.ApiResponse` <br/>
> `deliverynote_restore`(_api::`DeliveryNoteApi`, response_stream::`Channel`, `delivery_note_id`::`String`; _mediaType=nothing) -> `Channel`{ `DeliveryNote` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`DeliveryNoteApi`** | API context | 
**`delivery_note_id`** | **`String`** |  |

### Return type

[**`DeliveryNote`**](DeliveryNote.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **download_delivery_note_pdf**
> `download_delivery_note_pdf`(_api::`DeliveryNoteApi`, `delivery_note_id`::`String`; _mediaType=nothing) -> `Nothing`, `OpenAPI.Clients.ApiResponse` <br/>
> `download_delivery_note_pdf`(_api::`DeliveryNoteApi`, response_stream::`Channel`, `delivery_note_id`::`String`; _mediaType=nothing) -> `Channel`{ `Nothing` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`DeliveryNoteApi`** | API context | 
**`delivery_note_id`** | **`String`** |  |

### Return type

`Nothing`

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/pdf, application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **get_delivery_note**
> `get_delivery_note`(_api::`DeliveryNoteApi`, `delivery_note_id`::`String`; _mediaType=nothing) -> `DeliveryNote`, `OpenAPI.Clients.ApiResponse` <br/>
> `get_delivery_note`(_api::`DeliveryNoteApi`, response_stream::`Channel`, `delivery_note_id`::`String`; _mediaType=nothing) -> `Channel`{ `DeliveryNote` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`DeliveryNoteApi`** | API context | 
**`delivery_note_id`** | **`String`** |  |

### Return type

[**`DeliveryNote`**](DeliveryNote.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **list_delivery_notes**
> `list_delivery_notes`(_api::`DeliveryNoteApi`; `page`=nothing, `page_size`=nothing, `search`=nothing, `include_deleted`=nothing, _mediaType=nothing) -> `Vector{DeliveryNote}`, `OpenAPI.Clients.ApiResponse` <br/>
> `list_delivery_notes`(_api::`DeliveryNoteApi`, response_stream::`Channel`; `page`=nothing, `page_size`=nothing, `search`=nothing, `include_deleted`=nothing, _mediaType=nothing) -> `Channel`{ `Vector{DeliveryNote}` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`DeliveryNoteApi`** | API context | 

### Optional Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **`page`** | **`Int64`** |  | [default to nothing]
 **`page_size`** | **`Int64`** |  | [default to nothing]
 **`search`** | **`String`** |  | [default to nothing]
 **`include_deleted`** | **`Bool`** | Soft-delete entities: set true to include rows with &#x60;deleted_at&#x60; set. | [default to nothing]

### Return type

[**`Vector{DeliveryNote}`**](DeliveryNote.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **pursue_delivery_note**
> `pursue_delivery_note`(_api::`DeliveryNoteApi`, `delivery_note_id`::`String`; _mediaType=nothing) -> `Invoice`, `OpenAPI.Clients.ApiResponse` <br/>
> `pursue_delivery_note`(_api::`DeliveryNoteApi`, response_stream::`Channel`, `delivery_note_id`::`String`; _mediaType=nothing) -> `Channel`{ `Invoice` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`DeliveryNoteApi`** | API context | 
**`delivery_note_id`** | **`String`** |  |

### Return type

[**`Invoice`**](Invoice.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

