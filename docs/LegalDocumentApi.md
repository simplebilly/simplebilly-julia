# LegalDocumentApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_legal_documents**](LegalDocumentApi.md#get_legal_documents) | **GET** /api/v1/legal/documents | List all legal documents of the tenant. Missing documents are seeded from the default texts (with tenant placeholders replaced) on first access.
[**reset_legal_documents**](LegalDocumentApi.md#reset_legal_documents) | **POST** /api/v1/legal/documents/reset | Restore default texts for all documents (or a single doc_type/lang when the optional filter is given). Returns the full tenant list.
[**upsert_legal_documents**](LegalDocumentApi.md#upsert_legal_documents) | **PUT** /api/v1/legal/documents | Upsert legal documents per (doc_type, lang). Returns the full tenant list.


# **get_legal_documents**
> `get_legal_documents`(_api::`LegalDocumentApi`; _mediaType=nothing) -> `Vector{LegalDocument}`, `OpenAPI.Clients.ApiResponse` <br/>
> `get_legal_documents`(_api::`LegalDocumentApi`, response_stream::`Channel`; _mediaType=nothing) -> `Channel`{ `Vector{LegalDocument}` }, `OpenAPI.Clients.ApiResponse`

List all legal documents of the tenant. Missing documents are seeded from the default texts (with tenant placeholders replaced) on first access.

### Required Parameters
This endpoint does not need any parameter.

### Return type

[**`Vector{LegalDocument}`**](LegalDocument.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **reset_legal_documents**
> `reset_legal_documents`(_api::`LegalDocumentApi`, `legal_document_reset`::`LegalDocumentReset`; _mediaType=nothing) -> `Vector{LegalDocument}`, `OpenAPI.Clients.ApiResponse` <br/>
> `reset_legal_documents`(_api::`LegalDocumentApi`, response_stream::`Channel`, `legal_document_reset`::`LegalDocumentReset`; _mediaType=nothing) -> `Channel`{ `Vector{LegalDocument}` }, `OpenAPI.Clients.ApiResponse`

Restore default texts for all documents (or a single doc_type/lang when the optional filter is given). Returns the full tenant list.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`LegalDocumentApi`** | API context | 
**`legal_document_reset`** | [**`LegalDocumentReset`**](LegalDocumentReset.md) |  |

### Return type

[**`Vector{LegalDocument}`**](LegalDocument.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **upsert_legal_documents**
> `upsert_legal_documents`(_api::`LegalDocumentApi`, `legal_document_upsert`::`Vector{LegalDocumentUpsert}`; _mediaType=nothing) -> `Vector{LegalDocument}`, `OpenAPI.Clients.ApiResponse` <br/>
> `upsert_legal_documents`(_api::`LegalDocumentApi`, response_stream::`Channel`, `legal_document_upsert`::`Vector{LegalDocumentUpsert}`; _mediaType=nothing) -> `Channel`{ `Vector{LegalDocument}` }, `OpenAPI.Clients.ApiResponse`

Upsert legal documents per (doc_type, lang). Returns the full tenant list.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`LegalDocumentApi`** | API context | 
**`legal_document_upsert`** | [**`Vector{LegalDocumentUpsert}`**](LegalDocumentUpsert.md) |  |

### Return type

[**`Vector{LegalDocument}`**](LegalDocument.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

