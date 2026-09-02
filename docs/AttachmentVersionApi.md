# AttachmentVersionApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_attachment_version**](AttachmentVersionApi.md#create_attachment_version) | **POST** /api/v1/attachments/{attachment_id}/versions | 
[**list_attachment_versions**](AttachmentVersionApi.md#list_attachment_versions) | **GET** /api/v1/attachments/{attachment_id}/versions | 
[**restore_attachment_version**](AttachmentVersionApi.md#restore_attachment_version) | **POST** /api/v1/attachments/{attachment_id}/versions/{version_id}/restore | 


# **create_attachment_version**
> `create_attachment_version`(_api::`AttachmentVersionApi`, `attachment_id`::`String`, `new_version_request`::`NewVersionRequest`; _mediaType=nothing) -> `AttachmentVersion`, `OpenAPI.Clients.ApiResponse` <br/>
> `create_attachment_version`(_api::`AttachmentVersionApi`, response_stream::`Channel`, `attachment_id`::`String`, `new_version_request`::`NewVersionRequest`; _mediaType=nothing) -> `Channel`{ `AttachmentVersion` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`AttachmentVersionApi`** | API context | 
**`attachment_id`** | **`String`** |  |
**`new_version_request`** | [**`NewVersionRequest`**](NewVersionRequest.md) |  |

### Return type

[**`AttachmentVersion`**](AttachmentVersion.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **list_attachment_versions**
> `list_attachment_versions`(_api::`AttachmentVersionApi`, `attachment_id`::`String`; _mediaType=nothing) -> `Vector{AttachmentVersion}`, `OpenAPI.Clients.ApiResponse` <br/>
> `list_attachment_versions`(_api::`AttachmentVersionApi`, response_stream::`Channel`, `attachment_id`::`String`; _mediaType=nothing) -> `Channel`{ `Vector{AttachmentVersion}` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`AttachmentVersionApi`** | API context | 
**`attachment_id`** | **`String`** |  |

### Return type

[**`Vector{AttachmentVersion}`**](AttachmentVersion.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **restore_attachment_version**
> `restore_attachment_version`(_api::`AttachmentVersionApi`, `attachment_id`::`String`, `version_id`::`String`; _mediaType=nothing) -> `Attachment`, `OpenAPI.Clients.ApiResponse` <br/>
> `restore_attachment_version`(_api::`AttachmentVersionApi`, response_stream::`Channel`, `attachment_id`::`String`, `version_id`::`String`; _mediaType=nothing) -> `Channel`{ `Attachment` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`AttachmentVersionApi`** | API context | 
**`attachment_id`** | **`String`** |  |
**`version_id`** | **`String`** |  |

### Return type

[**`Attachment`**](Attachment.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

