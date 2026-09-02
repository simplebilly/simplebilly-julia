# AttachmentApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**attachment_restore**](AttachmentApi.md#attachment_restore) | **POST** /api/v1/attachments/{id}/restore | 
[**create_attachment**](AttachmentApi.md#create_attachment) | **POST** /api/v1/attachments | 
[**delete_attachment**](AttachmentApi.md#delete_attachment) | **DELETE** /api/v1/attachments/{id} | 
[**get_attachment**](AttachmentApi.md#get_attachment) | **GET** /api/v1/attachments/{id} | 
[**list_attachments**](AttachmentApi.md#list_attachments) | **GET** /api/v1/attachments/ | 
[**save_attachment_ocr_text**](AttachmentApi.md#save_attachment_ocr_text) | **PUT** /api/v1/attachments/{attachment_id}/ocr-text | Persist client-side OCR output for an attachment.


# **attachment_restore**
> `attachment_restore`(_api::`AttachmentApi`, `id`::`String`; _mediaType=nothing) -> `Attachment`, `OpenAPI.Clients.ApiResponse` <br/>
> `attachment_restore`(_api::`AttachmentApi`, response_stream::`Channel`, `id`::`String`; _mediaType=nothing) -> `Channel`{ `Attachment` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`AttachmentApi`** | API context | 
**`id`** | **`String`** |  |

### Return type

[**`Attachment`**](Attachment.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **create_attachment**
> `create_attachment`(_api::`AttachmentApi`, `attachment_create`::`AttachmentCreate`; _mediaType=nothing) -> `Attachment`, `OpenAPI.Clients.ApiResponse` <br/>
> `create_attachment`(_api::`AttachmentApi`, response_stream::`Channel`, `attachment_create`::`AttachmentCreate`; _mediaType=nothing) -> `Channel`{ `Attachment` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`AttachmentApi`** | API context | 
**`attachment_create`** | [**`AttachmentCreate`**](AttachmentCreate.md) |  |

### Return type

[**`Attachment`**](Attachment.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **delete_attachment**
> `delete_attachment`(_api::`AttachmentApi`, `id`::`String`; _mediaType=nothing) -> `Nothing`, `OpenAPI.Clients.ApiResponse` <br/>
> `delete_attachment`(_api::`AttachmentApi`, response_stream::`Channel`, `id`::`String`; _mediaType=nothing) -> `Channel`{ `Nothing` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`AttachmentApi`** | API context | 
**`id`** | **`String`** |  |

### Return type

`Nothing`

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **get_attachment**
> `get_attachment`(_api::`AttachmentApi`, `id`::`String`; _mediaType=nothing) -> `Attachment`, `OpenAPI.Clients.ApiResponse` <br/>
> `get_attachment`(_api::`AttachmentApi`, response_stream::`Channel`, `id`::`String`; _mediaType=nothing) -> `Channel`{ `Attachment` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`AttachmentApi`** | API context | 
**`id`** | **`String`** |  |

### Return type

[**`Attachment`**](Attachment.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **list_attachments**
> `list_attachments`(_api::`AttachmentApi`; `page`=nothing, `page_size`=nothing, `contact_id`=nothing, _mediaType=nothing) -> `Vector{Attachment}`, `OpenAPI.Clients.ApiResponse` <br/>
> `list_attachments`(_api::`AttachmentApi`, response_stream::`Channel`; `page`=nothing, `page_size`=nothing, `contact_id`=nothing, _mediaType=nothing) -> `Channel`{ `Vector{Attachment}` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`AttachmentApi`** | API context | 

### Optional Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **`page`** | **`Int64`** |  | [default to nothing]
 **`page_size`** | **`Int64`** |  | [default to nothing]
 **`contact_id`** | **`String`** |  | [default to nothing]

### Return type

[**`Vector{Attachment}`**](Attachment.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **save_attachment_ocr_text**
> `save_attachment_ocr_text`(_api::`AttachmentApi`, `attachment_id`::`String`, `ocr_text_request`::`OcrTextRequest`; _mediaType=nothing) -> `Attachment`, `OpenAPI.Clients.ApiResponse` <br/>
> `save_attachment_ocr_text`(_api::`AttachmentApi`, response_stream::`Channel`, `attachment_id`::`String`, `ocr_text_request`::`OcrTextRequest`; _mediaType=nothing) -> `Channel`{ `Attachment` }, `OpenAPI.Clients.ApiResponse`

Persist client-side OCR output for an attachment.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`AttachmentApi`** | API context | 
**`attachment_id`** | **`String`** |  |
**`ocr_text_request`** | [**`OcrTextRequest`**](OcrTextRequest.md) |  |

### Return type

[**`Attachment`**](Attachment.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

