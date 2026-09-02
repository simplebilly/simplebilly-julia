# ContactApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**contact_schema**](ContactApi.md#contact_schema) | **GET** /api/v1/contacts/schema | Serve JSON Schema for client-side validation
[**contact_timeline**](ContactApi.md#contact_timeline) | **GET** /api/v1/contacts/{contact_id}/timeline | Get the full per-contact timeline (Xentral §4.6/4.7).
[**create_contact**](ContactApi.md#create_contact) | **POST** /api/v1/contacts | Create contact
[**delete_contact**](ContactApi.md#delete_contact) | **DELETE** /api/v1/contacts/{contact_id} | Soft-delete contact
[**get_contact**](ContactApi.md#get_contact) | **GET** /api/v1/contacts/{contact_id} | Get single contact
[**list_contacts**](ContactApi.md#list_contacts) | **GET** /api/v1/contacts | List contacts with search, type filter, and pagination
[**sales_volume**](ContactApi.md#sales_volume) | **GET** /api/v1/contacts/sales-volume | Sales volume per contact
[**update_contact**](ContactApi.md#update_contact) | **PUT** /api/v1/contacts/{contact_id} | Update contact


# **contact_schema**
> `contact_schema`(_api::`ContactApi`; _mediaType=nothing) -> `Any`, `OpenAPI.Clients.ApiResponse` <br/>
> `contact_schema`(_api::`ContactApi`, response_stream::`Channel`; _mediaType=nothing) -> `Channel`{ `Any` }, `OpenAPI.Clients.ApiResponse`

Serve JSON Schema for client-side validation

### Required Parameters
This endpoint does not need any parameter.

### Return type

**`Any`**

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **contact_timeline**
> `contact_timeline`(_api::`ContactApi`, `contact_id`::`String`; _mediaType=nothing) -> `ContactTimelineResponse`, `OpenAPI.Clients.ApiResponse` <br/>
> `contact_timeline`(_api::`ContactApi`, response_stream::`Channel`, `contact_id`::`String`; _mediaType=nothing) -> `Channel`{ `ContactTimelineResponse` }, `OpenAPI.Clients.ApiResponse`

Get the full per-contact timeline (Xentral §4.6/4.7).

Aggregates communications, quotations, orders, invoices and uploaded documents for a contact, merged into a single reverse-chronological feed.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ContactApi`** | API context | 
**`contact_id`** | **`String`** |  |

### Return type

[**`ContactTimelineResponse`**](ContactTimelineResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **create_contact**
> `create_contact`(_api::`ContactApi`, `body`::`Any`; _mediaType=nothing) -> `Contact`, `OpenAPI.Clients.ApiResponse` <br/>
> `create_contact`(_api::`ContactApi`, response_stream::`Channel`, `body`::`Any`; _mediaType=nothing) -> `Channel`{ `Contact` }, `OpenAPI.Clients.ApiResponse`

Create contact

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ContactApi`** | API context | 
**`body`** | **`Any`** |  |

### Return type

[**`Contact`**](Contact.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **delete_contact**
> `delete_contact`(_api::`ContactApi`, `contact_id`::`String`; _mediaType=nothing) -> `Nothing`, `OpenAPI.Clients.ApiResponse` <br/>
> `delete_contact`(_api::`ContactApi`, response_stream::`Channel`, `contact_id`::`String`; _mediaType=nothing) -> `Channel`{ `Nothing` }, `OpenAPI.Clients.ApiResponse`

Soft-delete contact

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ContactApi`** | API context | 
**`contact_id`** | **`String`** |  |

### Return type

`Nothing`

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **get_contact**
> `get_contact`(_api::`ContactApi`, `contact_id`::`String`; _mediaType=nothing) -> `Contact`, `OpenAPI.Clients.ApiResponse` <br/>
> `get_contact`(_api::`ContactApi`, response_stream::`Channel`, `contact_id`::`String`; _mediaType=nothing) -> `Channel`{ `Contact` }, `OpenAPI.Clients.ApiResponse`

Get single contact

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ContactApi`** | API context | 
**`contact_id`** | **`String`** |  |

### Return type

[**`Contact`**](Contact.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **list_contacts**
> `list_contacts`(_api::`ContactApi`; `page`=nothing, `page_size`=nothing, `search`=nothing, `contact_type`=nothing, `tag`=nothing, _mediaType=nothing) -> `Vector{Contact}`, `OpenAPI.Clients.ApiResponse` <br/>
> `list_contacts`(_api::`ContactApi`, response_stream::`Channel`; `page`=nothing, `page_size`=nothing, `search`=nothing, `contact_type`=nothing, `tag`=nothing, _mediaType=nothing) -> `Channel`{ `Vector{Contact}` }, `OpenAPI.Clients.ApiResponse`

List contacts with search, type filter, and pagination

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ContactApi`** | API context | 

### Optional Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **`page`** | **`Int64`** |  | [default to nothing]
 **`page_size`** | **`Int64`** |  | [default to nothing]
 **`search`** | **`String`** |  | [default to nothing]
 **`contact_type`** | **`String`** |  | [default to nothing]
 **`tag`** | **`String`** |  | [default to nothing]

### Return type

[**`Vector{Contact}`**](Contact.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **sales_volume**
> `sales_volume`(_api::`ContactApi`; `page`=nothing, `page_size`=nothing, `search`=nothing, `contact_type`=nothing, `tag`=nothing, _mediaType=nothing) -> `SalesVolumeReport`, `OpenAPI.Clients.ApiResponse` <br/>
> `sales_volume`(_api::`ContactApi`, response_stream::`Channel`; `page`=nothing, `page_size`=nothing, `search`=nothing, `contact_type`=nothing, `tag`=nothing, _mediaType=nothing) -> `Channel`{ `SalesVolumeReport` }, `OpenAPI.Clients.ApiResponse`

Sales volume per contact

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ContactApi`** | API context | 

### Optional Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **`page`** | **`Int64`** |  | [default to nothing]
 **`page_size`** | **`Int64`** |  | [default to nothing]
 **`search`** | **`String`** |  | [default to nothing]
 **`contact_type`** | **`String`** |  | [default to nothing]
 **`tag`** | **`String`** |  | [default to nothing]

### Return type

[**`SalesVolumeReport`**](SalesVolumeReport.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **update_contact**
> `update_contact`(_api::`ContactApi`, `contact_id`::`String`, `body`::`Any`; _mediaType=nothing) -> `Contact`, `OpenAPI.Clients.ApiResponse` <br/>
> `update_contact`(_api::`ContactApi`, response_stream::`Channel`, `contact_id`::`String`, `body`::`Any`; _mediaType=nothing) -> `Channel`{ `Contact` }, `OpenAPI.Clients.ApiResponse`

Update contact

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ContactApi`** | API context | 
**`contact_id`** | **`String`** |  |
**`body`** | **`Any`** |  |

### Return type

[**`Contact`**](Contact.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

